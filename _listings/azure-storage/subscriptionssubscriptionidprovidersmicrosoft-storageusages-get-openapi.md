---
swagger: "2.0"
x-collection-name: Azure Storage
x-complete: 0
info:
  title: Azure Storage API Usage List
  version: 1.0.0
  description: Gets the current usage count and the limit for the resources under
    the subscription.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.Storage/usages:
    get:
      summary: Usage List
      description: Gets the current usage count and the limit for the resources under
        the subscription.
      operationId: Usage_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-storageusages-get
      parameters:
      - in: query
        name: No Name
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