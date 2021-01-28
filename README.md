# POC of using localstack's ES service endpoint and elastic's ES docker image

- `Dockerfile` is for building the Elasticsearch (from elastic.co) docker container
- `docker-compose` is to compose an AWS cloud stack using localstack, and a single node elasticsearch cluster
- `dc up` should bring up the stack

The reason we use both is because localstack only exposes the endpoints that the
[AWS ES Service](https://aws.amazon.com/elasticsearch-service/) accepts, but it's
not really a fully functioning elasticsearch cluster.
