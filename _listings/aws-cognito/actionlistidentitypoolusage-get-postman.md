{
  "info": {
    "name": "AWS Cognito API List Identity Pool Usage",
    "_postman_id": "7ca4e0fb-22d1-48de-9514-64c60a3f6fa1",
    "description": "Gets a list of identity pools registered with Cognito.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "92c1bc26-4699-49cc-8331-997436ca3403",
          "name": "createUserPool",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserPool?AdminCreateUserConfig=AdminCreateUserConfig&AliasAttributes=AliasAttributes&AutoVerifiedAttributes=AutoVerifiedAttributes&DeviceConfiguration=DeviceConfiguration&EmailConfiguration=EmailConfiguration&EmailVerificationMessage=EmailVerificationMessage&EmailVerificationSubject=EmailVerificationSubject&LambdaConfig=LambdaConfig&MfaConfiguration=MfaConfiguration&Policies=Policies&PoolName=PoolName&Schema=Schema&SmsAuthenticationMessage=SmsAuthenticationMessage&SmsConfiguration=SmsConfiguration&SmsVerificationMessage=SmsVerificationMessage&UserPoolTags=UserPoolTags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Cognito user pool and sets the password policy for the\n            pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "566830dd-0c9d-46b3-8d04-8f7259ed8c26"
            }
          ]
        },
        {
          "id": "676f93b8-f4d6-41cb-a964-9d1aac586f4d",
          "name": "deleteUserPool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserPool?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Amazon Cognito user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec1d1e74-12ef-4613-b329-ae9432a67ad3"
            }
          ]
        },
        {
          "id": "f8f262e9-8e79-492d-894b-b451c5dddc2f",
          "name": "deleteUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserPoolClient?ClientId=ClientId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows the developer to delete the user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5eccb988-1d76-4c2f-be4e-90119c6a5edf"
            }
          ]
        },
        {
          "id": "44a50ad2-7b85-4502-af61-cccaa893d66d",
          "name": "describeUserPool",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserPool?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the configuration information and metadata of the specified user\n            pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54a2d814-4652-4da2-912d-37664673f864"
            }
          ]
        },
        {
          "id": "fd2ad080-077c-47df-9794-9d1579d2174f",
          "name": "getDevice",
          "request": {
            "url": "http://example.com/api/?Action=GetDevice?AccessToken=AccessToken&DeviceKey=DeviceKey",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41bd023d-1d9f-4b4e-9f52-e6cdf077740e"
            }
          ]
        },
        {
          "id": "e61303a0-a48f-4a95-ac93-b93a3099214e",
          "name": "updateUserPool",
          "request": {
            "url": "http://example.com/api/?Action=UpdateUserPool?AdminCreateUserConfig=AdminCreateUserConfig&AutoVerifiedAttributes=AutoVerifiedAttributes&DeviceConfiguration=DeviceConfiguration&EmailConfiguration=EmailConfiguration&EmailVerificationMessage=EmailVerificationMessage&EmailVerificationSubject=EmailVerificationSubject&LambdaConfig=LambdaConfig&MfaConfiguration=MfaConfiguration&Policies=Policies&SmsAuthenticationMessage=SmsAuthenticationMessage&SmsConfiguration=SmsConfiguration&SmsVerificationMessage=SmsVerificationMessage&UserPoolId=UserPoolId&UserPoolTags=UserPoolTags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the specified user pool with the specified attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "054372c1-b21b-44e6-baca-f0d9c7c6e873"
            }
          ]
        }
      ]
    },
    {
      "name": "user Pools",
      "item": [
        {
          "id": "47a55dce-3b71-4a69-9279-a7d0e0596f70",
          "name": "listUserPools",
          "request": {
            "url": "http://example.com/api/?Action=ListUserPools?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the user pools associated with an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a7d4ad2-8d1c-496c-859f-de0048354d2e"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity Pools",
      "item": [
        {
          "id": "f98b7889-12ef-46b9-bd43-6d7a980e7dc5",
          "name": "getIdentityPoolConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityPoolConfiguration?IdentityPoolId=IdentityPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the configuration settings of an identity pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5363aaa6-746b-4fac-a1ea-55f4a4657cc5"
            }
          ]
        },
        {
          "id": "6672acc4-e9a9-4457-8a25-5be4cc3d0e37",
          "name": "listIdentityPoolUsage",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentityPoolUsage?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of identity pools registered with Cognito."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89b80900-f825-4821-b645-5367d7d357a5"
            }
          ]
        }
      ]
    }
  ]
}