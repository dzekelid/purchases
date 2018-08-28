swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PurchaseReservedDBInstancesOffering:
    get:
      summary: Purchase Reserved D B Instances Offering
      description: Purchases a reserved DB instance offering.
      operationId: purchasereserveddbinstancesoffering
      x-api-path-slug: actionpurchasereserveddbinstancesoffering-get
      parameters:
      - in: query
        name: DBInstanceCount
        description: The number of instances to reserve
        type: string
      - in: query
        name: ReservedDBInstanceId
        description: Customer-specified identifier to track this reservation
        type: string
      - in: query
        name: ReservedDBInstancesOfferingId
        description: The ID of the Reserved DB instance offering to purchase
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances