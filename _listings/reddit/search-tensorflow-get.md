---
swagger: "2.0"
info:
  title: Reddit Search for Tensorflow
  description: Searching for Tensorflow
  version: 1.0.0
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search.json:
    get:
      summary: Search for Tensorflow
      description: Searching Reddit for Tensorflow
      operationId: search
      parameters:
      - in: query
        name: q
        description: The query.
        type: string
        default: Kafka
      responses:
        200:
          description: OK
      tags:
      - Search
---
