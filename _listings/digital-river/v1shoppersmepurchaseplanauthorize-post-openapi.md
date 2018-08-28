---
swagger: "2.0"
x-collection-name: Digital River
x-complete: 0
info:
  title: Digital River Shopper API Post Shoppers Me Purchase Plan Authorize
  description: Post shoppers me purchase plan authorize.
  version: v1
host: store.digitalriver.com
basePath: /store/{mysite}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/shoppers/me/products/{id}/purchase:
    post:
      summary: Post Shoppers Me Products Purchase
      description: Post shoppers me products purchase.
      operationId: postV1ShoppersMeProductsPurchase
      x-api-path-slug: v1shoppersmeproductsidpurchase-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Products
      - Purchase
  /v1/shoppers/me/purchase-plan/authorize:
    post:
      summary: Post Shoppers Me Purchase Plan Authorize
      description: Post shoppers me purchase plan authorize.
      operationId: postV1ShoppersMePurchasePlanAuthorize
      x-api-path-slug: v1shoppersmepurchaseplanauthorize-post
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Purchase
      - Plan
      - Authorize
  /v1/shoppers/me/purchase-plan/search:
    get:
      summary: Get Shoppers Me Purchase Plan Search
      description: Get shoppers me purchase plan search.
      operationId: getV1ShoppersMePurchasePlanSearch
      x-api-path-slug: v1shoppersmepurchaseplansearch-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Purchase
      - Plan
      - Search
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