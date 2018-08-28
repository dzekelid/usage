swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /library/usage/{mediaId}:
    get:
      summary: Get Library Item Usage Report
      description: Get the records for the library item usage report
      operationId: libraryUsageReport
      x-api-path-slug: libraryusagemediaid-get
      responses:
        200:
          description: OK
      tags:
      - Library
      - Item
      - Usage
      - Report
  /library/usage/layouts/{mediaId}:
    get:
      summary: Get Library Item Usage Report for Layouts
      description: Get the records for the library item usage report for Layouts
      operationId: libraryUsageLayoutsReport
      x-api-path-slug: libraryusagelayoutsmediaid-get
      responses:
        200:
          description: OK
      tags:
      - Library
      - Item
      - Usage
      - ReportLayouts