---
swagger: "2.0"
x-collection-name: Azure Storage
x-complete: 1
info:
  title: StorSimpleSeries8000ManagementClient
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
---