swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
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
  /?Action=ListIdentityPoolUsage:
    get:
      summary: List Identity Pool Usage
      description: Gets a list of identity pools registered with Cognito.
      operationId: listIdentityPoolUsage
      x-api-path-slug: actionlistidentitypoolusage-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of results to be returned
        type: string
      - in: query
        name: NextToken
        description: A pagination token for obtaining the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pools