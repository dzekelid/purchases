---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Purchaseasset
  version: 1.0.0
  description: Add api purchaseasset.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/PurchaseAsset:
    post:
      summary: Add API Purchaseasset
      description: Add api purchaseasset.
      operationId: ApiPurchaseAssetPost
      x-api-path-slug: apipurchaseasset-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Purchaseasset
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