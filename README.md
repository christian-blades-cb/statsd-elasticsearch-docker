# statsd-elasticsearch #

Timings and tallies collection. Into elasticsearch. For great analytics.

Also, Docker.

## How to

### The easy way

* clone this repository
* `docker-compose up`

### The other way

`docker run` this image and provide a few environment variables

* `ES_PORT_9200_TCP_ADDR` - hostname/ip of the elasticsearch host (defaults to docker host... usually)
* `ES_PORT_9200_TCP_PORT` - port number that elasticsearch (defaults to 9200)
* `ES_PATH` - path to elasticsearch, in case you have it behind a reverse proxy or something (defaults to "/")
* `ES_PREFIX` - index prefix for the statsd documents, ex: `statsd-2015.03.25` (defaults to "statsd")
