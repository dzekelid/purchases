swagger: "2.0"
x-collection-name: Getty Images
x-complete: 1
info:
  title: Getty Images
  description: build-applications-using-the-worlds-most-powerful-imagery
  version: 1.0.0
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
      summary: Get Purchased Images
      description: "This endpoint returns a list of all assets purchased on gettyimages.com
        by the username used for authentication. \r\nUse of this endpoint requires
        configuration changes to your API key. \r\nPlease contact [developersupport@gettyimages.com](mailto:developersupport@gettyimages.com)
        to learn more.\r\n\r\nYou'll need an API key and access token to use this
        resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
        for more information on how to sign up for an API key."
      operationId: Purchases_GetPreviousAssetPurchases
      x-api-path-slug: v3purchasedassets-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: end_date
        description: If specified, retrieves previous purchases on or before this
          date
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: start_date
        description: If specified, retrieves previous purchases on or after this date
      responses:
        200:
          description: OK
      tags:
      - Images
      - Purchases
  /v3/purchased-images:
    get:
      summary: Get Previously Purchased Images
      description: "This endpoint returns a list of all images purchased on gettyimages.com
        by the username used for authentication.\r\nUse of this endpoint requires
        configuration changes to your API key. Please contact [developersupport@gettyimages.com](mailto:developersupport@gettyimages.com)\r\nto
        learn more.\r\n\r\nYou'll need an API key and access token to use this resource.
        Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
        for more information on how to sign up for an API key."
      operationId: Purchases_GetPreviousPurchases
      x-api-path-slug: v3purchasedimages-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: end_date
        description: If specified, retrieves previous purchases on or before this
          date
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: start_date
        description: If specified, retrieves previous purchases on or after this date
      responses:
        200:
          description: OK
      tags:
      - Images
      - Purchases