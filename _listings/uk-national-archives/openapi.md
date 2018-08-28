swagger: "2.0"
x-collection-name: UK National Archives
x-complete: 1
info:
  title: Getty Images
  description: build-applications-using-the-worlds-most-powerful-imagery
  version: "3.0"
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/purchased-assets:
    get:
      summary: Get Purchased Assets
      description: Get previously purchased images and video.
      operationId: getV3PurchasedAssets
      x-api-path-slug: v3purchasedassets-get
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: date_from
        description: If specified, retrieves previous purchases on or after this date
      - in: query
        name: date_to
        description: If specified, retrieves previous purchases on or before this
          date
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      responses:
        200:
          description: OK
      tags:
      - Purchased
      - Assets
  /v3/purchased-images:
    get:
      summary: Get Purchased Images
      description: Get previously purchased images.
      operationId: getV3PurchasedImages
      x-api-path-slug: v3purchasedimages-get
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: date_from
        description: If specified, retrieves previous purchases on or after this date
      - in: query
        name: date_to
        description: If specified, retrieves previous purchases on or before this
          date
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      responses:
        200:
          description: OK
      tags:
      - Purchased
      - Images