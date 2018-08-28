---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Get Library Item Usage Report for Layouts
  description: Get the records for the library item usage report for Layouts
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