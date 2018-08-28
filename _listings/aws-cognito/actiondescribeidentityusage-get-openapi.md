---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Describe Identity Usage
  version: 1.0.0
  description: Gets usage information for an identity, including number of datasets
    and data usage.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeIdentityPoolUsage:
    get:
      summary: Describe Identity Pool Usage
      description: Gets usage details (for example, data storage) about a particular
        identity pool.
      operationId: describeIdentityPoolUsage
      x-api-path-slug: actiondescribeidentitypoolusage-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool Usage
  /?Action=DescribeIdentityUsage:
    get:
      summary: Describe Identity Usage
      description: Gets usage information for an identity, including number of datasets
        and data usage.
      operationId: describeIdentityUsage
      x-api-path-slug: actiondescribeidentityusage-get
      parameters:
      - in: query
        name: IdentityId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool Usage
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