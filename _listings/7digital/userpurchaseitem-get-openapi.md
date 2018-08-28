---
swagger: "2.0"
x-collection-name: 7digital
x-complete: 0
info:
  title: 7digital Purchasing API user/purchase/item
  description: This method allows a user to purchase an item at the price as advertised
    on 7digital.com. It will return the download URL of each item purchased. For example,
    if a release consisting of multiple tracks was purchased, then the download URL
    of each item constituting the release will be returned.nttttttFor a user purchase
    to be processed, the user should already have a default debit or credit card set
    up for payments.ntttThis method allows users to take advantage of 7digital.com
    promotional offers and is only available to selected partners building 7digital
    branded integrations. For white-label integrations please use user/purchase/rrpItem
    or user/purchase/pricedItem.
  version: "1.2"
host: api.7digital.com
basePath: 1.2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  user/purchase/basket:
    'get ':
      summary: user/purchase/basket
      description: This method allows a user to purchase a basket with items that
        have been added via basket/additem or basket/addpriceditem. It will return
        the download URL of each item purchased. For example, if a release consisting
        of multiple tracks was purchased, then the download URL of each item constituting
        the release will be returned.
      operationId: userpurchasebasket
      x-api-path-slug: userpurchasebasket-get
      parameters:
      - ~
      - in: query
        name: basketid
        description: This is the session ID for the basket that contains the items
          to purchase
      - in: query
        name: country
        description: nttttttttThe country that all basket items were selected from
      - in: query
        name: oauth_token
        description: users OAuth accesstoken
      - in: query
        name: shopid
        description: nttttttttThe shop ID that all basket items were selected from
      - in: query
        name: tag_*key*
        description: nttttttttAdditional data to be stored with successful transactions,
          for the purposes such as tagging affiliated or marketing information
      responses:
        200:
          description: OK
      tags:
      - User
      - Purchase
      - Basket
  user/purchase/item:
    'get ':
      summary: user/purchase/item
      description: This method allows a user to purchase an item at the price as advertised
        on 7digital.com. It will return the download URL of each item purchased. For
        example, if a release consisting of multiple tracks was purchased, then the
        download URL of each item constituting the release will be returned.nttttttFor
        a user purchase to be processed, the user should already have a default debit
        or credit card set up for payments.ntttThis method allows users to take advantage
        of 7digital.com promotional offers and is only available to selected partners
        building 7digital branded integrations. For white-label integrations please
        use user/purchase/rrpItem or user/purchase/pricedItem.
      operationId: userpurchaseitem
      x-api-path-slug: userpurchaseitem-get
      parameters:
      - ~
      - in: query
        name: country
        description: The code of the country the end user resides in
      - in: query
        name: oauth_token
        description: users OAuth accesstoken
      - in: query
        name: price
        description: nttttttttThe price that has been displayed to the user prior
          to purchase
      - in: query
        name: releaseId
        description: The unique ID of the release being purchased
      - in: query
        name: shopid
        description: nttttttttThe shop ID that all basket items were selected from
      - in: query
        name: tag_*key*
        description: nttttttttAdditional data to be stored with successful transactions,
          for the purposes such as tagging affiliated or marketing information
      - in: query
        name: trackId
        description: The unique ID of the track being purchased
      responses:
        200:
          description: OK
      tags:
      - User
      - Purchase
      - Item
  user/purchase/rrpItem:
    'get ':
      summary: user/purchase/rrpItem
      description: This method allows a user to purchase an item at 7digital recommended
        retail price (RRP). It will return the download URL of each item purchased.
        For example, if a release consisting of multiple tracks was purchased, then
        the download URL of each item constituting the release will be returned.nttttttFor
        a user purchase to be processed, the user should already have a default debit
        or credit card set up for payments.
      operationId: userpurchaserrpitem
      x-api-path-slug: userpurchaserrpitem-get
      parameters:
      - ~
      - in: query
        name: country
        description: nttttttttThe country that all basket items were selected from
      - in: query
        name: oauth_token
        description: users OAuth accesstoken
      - in: query
        name: price
        description: nttttttttThe price that has been displayed to the user prior
          to purchase
      - in: query
        name: releaseId
        description: The unique ID of the release being purchased
      - in: query
        name: shopid
        description: nttttttttThe shop ID that all basket items were selected from
      - in: query
        name: tag_*key*
        description: nttttttttAdditional data to be stored with successful transactions,
          for the purposes such as tagging affiliated or marketing information
      - in: query
        name: trackId
        description: The unique ID of the track being purchased
      responses:
        200:
          description: OK
      tags:
      - User
      - Purchase
      - RrpItem
  user/purchase/{purchaseid}/track/{trackid}:
    'delete ':
      summary: user/purchase/{purchaseid}/track/{trackid}
      description: This method allows a user to remove a purchase of a track from
        the sales report when the purchase has been refunded.
      operationId: userpurchasepurchaseidtracktrackid
      x-api-path-slug: userpurchasepurchaseidtracktrackid-delete
      parameters:
      - ~
      - in: query
        name: purchaseid
        description: purchase id identifying the transaction at 7digitals end that
          the refunded item belongs to
      - in: query
        name: trackid
        description: nttttttttThe 7digital id of the track being refundednnttttttt
      responses:
        200:
          description: OK
      tags:
      - User
      - Purchase
      - Purchaseid
      - Track
      - Trackid
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