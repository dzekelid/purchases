swagger: "2.0"
x-collection-name: Intuit
x-complete: 1
info:
  title: QuickBooks Online V3 API
  description: the-quickbooks-online-accounting-api-is-a-restful-api-that-is-used-to-access-quickbooks-companies-docs-
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /purchase:
    post:
      summary: Post Purchase
      description: |-
        Create a puchase object
        Method : POST
      operationId: postPurchase
      x-api-path-slug: purchase-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Purchase
  /purchaseorder/178:
    get:
      summary: Get Purchase Order
      description: |-
        Read a puchase-order object
        Method : POST
      operationId: getPurchaseorder178
      x-api-path-slug: purchaseorder178-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Purchase
      - Order
  /purchase/175:
    get:
      summary: Get Purchase
      description: |-
        Read a puchase object by Id
        Method : POST
      operationId: getPurchase175
      x-api-path-slug: purchase175-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Purchase
  /purchaseorder:
    post:
      summary: Post Purchase Order
      description: |-
        Create a puchase-order object
        Method : POST
      operationId: postPurchaseorder
      x-api-path-slug: purchaseorder-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Purchase
      - Order