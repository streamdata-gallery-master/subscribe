---
swagger: "2.0"
info:
  title: Reddit Search for React
  description: Searching for React
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
      summary: Search for React
      description: Searching Reddit for React
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
