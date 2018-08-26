---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/templateusagecount:
    get:
      summary: Get the usage count for a template in envelopes
      description: Get the usage count for a template in envelopes.
      operationId: DocumentGeneration_getDocumentSubTypesBytemplateId
      x-api-path-slug: apidocumentgenerationtemplateusagecount-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: templateId
      responses:
        200:
          description: OK
      tags:
      - Usage
      - Counta
      - Template
      - In
      - Envelopes
---