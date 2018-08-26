---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Add To SIP Credentials List
  description: Change the password of a Credential record.nnIf the change is successful,
    Twilio will respond with the Credential record but will not include the password
    in the response.n
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}/Credentials/{CredentialSid}:
    delete:
      summary: Delete SIP Credential From List
      description: Remove a Credential from a CredentialList.
      operationId: remove-a-credential-from-a-credentiallist
      x-api-path-slug: accountsaccountsidsipcredentiallistsclsidcredentialscredentialsid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CLSid
        description: A 34 character string that uniquely identifies the credential
          list
      - in: path
        name: CredentialSid
      responses:
        200:
          description: OK
      tags:
      - SIP Credential Lists
    get:
      summary: Get SIP Credentials List
      description: Get a specific Credential in a list. Though a password is stored
        for each username in your list, the password is not returned to protect your
        password. If you cannot remember your password, you will need to POST to this
        resource to update it.
      operationId: get-a-specific-credential-in-a-list-though-a-password-is-stored-for-each-username-in-your-list-the-p
      x-api-path-slug: accountsaccountsidsipcredentiallistsclsidcredentialscredentialsid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CLSid
        description: A 34 character string that uniquely identifies the credential
          list
      - in: path
        name: CredentialSid
      responses:
        200:
          description: OK
      tags:
      - SIP Credential Lists
    post:
      summary: Add To SIP Credentials List
      description: Change the password of a Credential record.nnIf the change is successful,
        Twilio will respond with the Credential record but will not include the password
        in the response.n
      operationId: change-the-password-of-a-credential-recordif-the-change-is-successful-twilio-will-respond-with-the-c
      x-api-path-slug: accountsaccountsidsipcredentiallistsclsidcredentialscredentialsid-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CLSid
        description: A 34 character string that uniquely identifies the credential
          list
      - in: path
        name: CredentialSid
      responses:
        200:
          description: OK
      tags:
      - SIP Credential Lists
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