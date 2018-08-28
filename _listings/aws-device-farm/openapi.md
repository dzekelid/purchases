swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 1
info:
  title: AWS Device Farm API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PurchaseOffering:
    get:
      summary: Purchase Offering
      description: Immediately purchases offerings for an AWS account.
      operationId: purchaseOffering
      x-api-path-slug: actionpurchaseoffering-get
      parameters:
      - in: query
        name: offeringId
        description: The ID of the offering
        type: string
      - in: query
        name: quantity
        description: The number of device slots you wish to purchase in an offering
          request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offerings