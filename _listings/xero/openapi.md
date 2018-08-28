swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Xero oAuth 1a
  description: a-collection-to-authenticate-to-the-xero-api-using-oauth1-0a
  version: 1.0.0
host: api.xero.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /PurchaseOrders/{PurchaseOrderID}:
    get:
      summary: Get Purchaseorders Purchaseorder
      description: Get purchaseorders purchaseorder.
      operationId: getPurchaseordersPurchaseorder
      x-api-path-slug: purchaseorderspurchaseorderid-get
      parameters:
      - in: path
        name: PurchaseOrderID
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders
      - PurchaseOrderID
    post:
      summary: Post Purchaseorders Purchaseorder
      description: Post purchaseorders purchaseorder.
      operationId: postPurchaseordersPurchaseorder
      x-api-path-slug: purchaseorderspurchaseorderid-post
      parameters:
      - in: path
        name: PurchaseOrderID
      - in: body
        name: PurchaseOrders
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders
      - PurchaseOrderID
    x-related-model:
      summary: X-related-model Purchaseorders Purchaseorder
      description: X-related-model purchaseorders purchaseorder.
      operationId: x-related-modelPurchaseordersPurchaseorder
      x-api-path-slug: purchaseorderspurchaseorderid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders
      - PurchaseOrderID
  /PurchaseOrders/{PurchaseOrderID}/Attachments:
    get:
      summary: Get Purchaseorders Purchaseorder Attachments
      description: Get purchaseorders purchaseorder attachments.
      operationId: getPurchaseordersPurchaseorderAttachments
      x-api-path-slug: purchaseorderspurchaseorderidattachments-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: PurchaseOrderID
        description: The Xero generated unique identifier for a purchase order
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders
      - PurchaseOrderID
      - Attachments
  /PurchaseOrders/{PurchaseOrderID}/Attachments/{FileName}:
    get:
      summary: Get Purchaseorders Purchaseorder Attachments Filename
      description: Get purchaseorders purchaseorder attachments filename.
      operationId: getPurchaseordersPurchaseorderAttachmentsFilename
      x-api-path-slug: purchaseorderspurchaseorderidattachmentsfilename-get
      parameters:
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      - in: path
        name: PurchaseOrderID
        description: The Xero generated unique identifier for a purchase order
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders
      - PurchaseOrderID
      - Attachments
      - FileName
    post:
      summary: Post Purchaseorders Purchaseorder Attachments Filename
      description: Post purchaseorders purchaseorder attachments filename.
      operationId: postPurchaseordersPurchaseorderAttachmentsFilename
      x-api-path-slug: purchaseorderspurchaseorderidattachmentsfilename-post
      parameters:
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      - in: path
        name: PurchaseOrderID
        description: The Xero generated unique identifier for a purchase order
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders
      - PurchaseOrderID
      - Attachments
      - FileName
  /PurchaseOrders:
    get:
      summary: Get Purchaseorders
      description: Get purchaseorders.
      operationId: getPurchaseorders
      x-api-path-slug: purchaseorders-get
      parameters:
      - in: query
        name: DateFrom
      - in: query
        name: DateTo
      - in: query
        name: No Name
      - in: query
        name: Status
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders
    post:
      summary: Post Purchaseorders
      description: Post purchaseorders.
      operationId: postPurchaseorders
      x-api-path-slug: purchaseorders-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: PurchaseOrders
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders
    put:
      summary: Put Purchaseorders
      description: Put purchaseorders.
      operationId: putPurchaseorders
      x-api-path-slug: purchaseorders-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: PurchaseOrders
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders
    x-related-model:
      summary: X-related-model Purchaseorders
      description: X-related-model purchaseorders.
      operationId: x-related-modelPurchaseorders
      x-api-path-slug: purchaseorders-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders