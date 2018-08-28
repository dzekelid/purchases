swagger: "2.0"
x-collection-name: Flowroute
x-complete: 1
info:
  title: Flowroute APIs
  description: the-flowroute-apis-are-organized-around-rest--our-apis-have-resourceoriented-urls-support-http-verbs-and-respond-with-http-status-codes--all-api-requests-and-responses-including-errors-will-be-represented-as-json-objects--you-can-use-the-flowroute-apis-to-manage-your-flowroute-phone-numbers-including-setting-primary-and-failover-routes-for-inbound-calls-and-sending-text-messages-sms-and-mms-using-longcode-or-tollfree-numbers-in-your-account-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/numbers/{id}:
    post:
      summary: Purchase a Phone Number
      description: Lets you purchase a phone number from available Flowroute inventory.
      operationId: lets-you-purchase-a-phone-number-from-available-flowroute-inventory
      x-api-path-slug: v2numbersid-post
      parameters:
      - in: path
        name: id
        description: Phone number to purchase
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Purchase
      - Phone
      - Number