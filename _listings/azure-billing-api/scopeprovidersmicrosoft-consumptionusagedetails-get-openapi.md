---
swagger: "2.0"
x-collection-name: Azure Billing API
x-complete: 0
info:
  title: Azure Billing API Usage Details List
  description: Lists the usage details for a scope in reverse chronological order
    by billing period. Usage details are available via this API only for January 1,
    2017 or later.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{scope}/providers/Microsoft.Consumption/usageDetails:
    get:
      summary: Usage Details List
      description: Lists the usage details for a scope in reverse chronological order
        by billing period. Usage details are available via this API only for January
        1, 2017 or later.
      operationId: UsageDetails_List
      x-api-path-slug: scopeprovidersmicrosoft-consumptionusagedetails-get
      parameters:
      - in: query
        name: $expand
        description: May be used to expand the additionalProperties or meterDetails
          property within a list of usage details
      - in: query
        name: $filter
        description: May be used to filter usageDetails by usageEnd (Utc time)
      - in: query
        name: $skiptoken
        description: Skiptoken is only used if a previous operation returned a partial
          result
      - in: query
        name: $top
        description: May be used to limit the number of results to the most recent
          N usageDetails
      - in: query
        name: No Name
      - in: path
        name: scope
        description: The scope of the usage details
      responses:
        200:
          description: OK
      tags:
      - Usage
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