---
swagger: "2.0"
x-collection-name: Flowroute
x-complete: 0
info:
  title: FlowRoute API Purchase a Phone Number
  description: Lets you purchase a phone number from available Flowroute inventory.
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