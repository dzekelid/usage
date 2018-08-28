swagger: "2.0"
x-collection-name: UK National Archives
x-complete: 1
info:
  title: Getty Images
  description: build-applications-using-the-worlds-most-powerful-imagery
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