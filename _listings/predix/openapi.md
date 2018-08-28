swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /health/memory:
    get:
      summary: Validate the EC service memory usage
      description: Validate the EC gateway memory usage
      operationId: validate-the-ec-gateway-memory-usage
      x-api-path-slug: healthmemory-get
      responses:
        200:
          description: Successful response
      tags:
      - Validate
      - EC
      - Service
      - Memory
      - Usage
  /reports/usage:
    post:
      summary: Report usage
      description: Report usage by zoneid
      operationId: report-usage-by-zoneid
      x-api-path-slug: reportsusage-post
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: body
        name: content
        description: The content for reporting the usage
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: predix-zone-id
        description: Cloud Foundry service instance id
      responses:
        200:
          description: Successful response
      tags:
      - Report
      - Usage
    get:
      summary: Get last usage
      description: get last usage by zoneid
      operationId: get-last-usage-by-zoneid
      x-api-path-slug: reportsusage-get
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: header
        name: predix-zone-id
        description: Cloud Foundry service instance id
      responses:
        200:
          description: Successful response
      tags:
      - Last
      - Usage
  /v1/tenants/{tenant_uuid}/usage:
    get:
      summary: Get Tenants Usage
      description: Get tenants usage.
      operationId: getV1TenantsTenantUuUsage
      x-api-path-slug: v1tenantstenant-uuidusage-get
      parameters:
      - in: query
        name: end_date
        description: end_date
      - in: query
        name: start_date
        description: start_date
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
      - Usage