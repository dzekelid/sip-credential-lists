{
  "info": {
    "name": "Twilio Get SIP Credentials List",
    "_postman_id": "d9d785a4-d14c-4d43-b4c5-000df838af45",
    "description": "Gets a list of Credential Lists for an account",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "sip credential lists",
      "item": [
        {
          "id": "24930cda-3a32-45c9-8861-e09003e3d765",
          "name": "gets-a-list-of-credential-lists-for-an-account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/SIP/CredentialLists"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of Credential Lists for an account"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"uri\": \"uri\",\r\n    \"firstpageuri\": \"firstpageuri\",\r\n    \"nextpageuri\": \"nextpageuri\",\r\n    \"previouspageuri\": \"previouspageuri\",\r\n    \"page\": \"page\",\r\n    \"pagesize\": \"pagesize\",\r\n    \"credential_list\": {}\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "9c8f6adf-8457-4847-8613-c350f91eda6d"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "The supplied credentials, if any, are not sufficient to access the resource",
              "code": 401,
              "name": "Response_401",
              "id": "c4568cdb-ef45-4ab3-9a9f-6a34aad9cbdc"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "You know this one",
              "code": 404,
              "name": "Response_404",
              "id": "7fd60c15-f1b4-458d-ad60-1c79c5be5a88"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "Your application is sending too many simultaneous requests",
              "code": 429,
              "name": "Response_429",
              "id": "b778325f-f384-421e-976c-3fe003ac76d7"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "We couldn't return the representation due to an internal server error",
              "code": 500,
              "name": "Response_500",
              "id": "45ef877a-331f-4c7f-ae6e-d4db22376a8e"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "We are temporarily unable to return the representation",
              "code": 503,
              "name": "Response_503",
              "id": "42ba6dbe-7414-4d14-b8b7-4ee0d93a1181"
            }
          ]
        }
      ]
    }
  ]
}