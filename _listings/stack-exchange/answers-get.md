---
swagger: "2.0"
info:
  title: Stack Exchange Answers
  description: Subscribe to Stack Overflow answers.
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /answers:
    get:
      summary: Get Answers
      description: Returns answers for Stack Overflow
      operationId: subscribeAnswers
      parameters:
      - in: query
        name: order
      - in: query
        name: site
        description: The site to return results for.
      - in: query
        name: sort
        default: activity
      - in: query
        name: tagged
        description: The tag to return.
      tags:
      - Answers
---
