---
swagger: "2.0"
x-collection-name: Azure Billing API
x-complete: 1
info:
  title: ConsumptionManagementClient
  description: consumption-management-client-provides-access-to-consumption-resources-for-azure-webdirect-subscriptions--other-subscription-types-which-were-not-purchased-directly-through-the-azure-web-portal-are-not-supported-through-this-preview-api-
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
---