---
swagger: "2.0"
info:
  title: Stack Exchange Questions
  description: Subscribe to Stack Overflow questions.
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
  /questions:
    get:
      summary: Get Questions
      description: Subscribe to questions from Stack Overflow.
      operationId: getQuestions
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
      - Questions
---
