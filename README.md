Elasticsearch using Docker images
===

### Run on the development env

```bash
$ sudo docker run -d -p 9200:9200 -e "path.conf=./config/development.yaml" elasticsearch:5

# see elasticsearch's version
$ curl -XGET http://127.0.0.1:9200/
{
  "name" : "davHqzx",
  "cluster_name" : "elasticsearch",
  "cluster_uuid" : "-ui9wy-iQgmIpnlHOkQ_gA",
  "version" : {
    "number" : "5.4.2",
    "build_hash" : "929b078",
    "build_date" : "2017-06-15T02:29:28.122Z",
    "build_snapshot" : false,
    "lucene_version" : "6.5.1"
  },
  "tagline" : "You Know, for Search"
}
```
