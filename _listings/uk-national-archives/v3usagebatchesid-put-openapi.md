---
swagger: "2.0"
x-collection-name: UK National Archives
x-complete: 0
info:
  title: Getty Images Search API Put Usage Batches
  description: Report usage of assets via a batch format..
  version: "3.0"
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/usage-batches/{id}:
    put:
      summary: Put Usage Batches
      description: Report usage of assets via a batch format..
      operationId: putV3UsageBatches
      x-api-path-slug: v3usagebatchesid-put
      parameters:
      - in: header
        name: Accept-Language
        description: Accept-Language parameter optional
      - in: header
        name: Authorization
        description: Authorization token required
      - in: path
        name: id
        description: Specifies a unique batch transaction id to identify the report
      - in: body
        name: request
        description: Specifies up to 1000 sets of asset Id, usage count, and date
          of use to submit usages for
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Usage
      - Batches
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---