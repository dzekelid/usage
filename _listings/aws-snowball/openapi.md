---
swagger: "2.0"
x-collection-name: AWS Snowball
x-complete: 1
info:
  title: AWS Snowball API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetSnowballUsage:
    get:
      summary: Get Snowball Usage
      description: |-
        Returns information about the Snowball service limit for your account, and also the
              number of Snowballs your account has in use.
      operationId: getSnowballUsage
      x-api-path-slug: actiongetsnowballusage-get
      parameters:
      - in: query
        name: SnowballLimit
        description: The service limit for number of Snowballs this account can have
          at once
        type: string
      - in: query
        name: SnowballsInUse
        description: The number of Snowballs that this account is currently using
        type: string
      responses:
        200:
          description: OK
      tags:
      - Usage
---