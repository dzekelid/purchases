swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PurchaseReservedInstancesOffering:
    get:
      summary: Purchase Reserved Instances Offering
      description: Purchases a Reserved Instance for use with your account.
      operationId: purchasereservedinstancesoffering
      x-api-path-slug: actionpurchasereservedinstancesoffering-get
      parameters:
      - in: query
        name: PrincipalArn
        description: The ARN of the principal, which can be an IAM role, IAM user,
          or the root user
        type: string
      - in: query
        name: Resource
        description: 'The type of resource: instance | reservation |        snapshot
          | volume'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instance
  /?Action=PurchaseScheduledInstances:
    get:
      summary: Purchase Scheduled Instances
      description: Purchases one or more Scheduled Instances with the specified schedule.
      operationId: purchasescheduledinstances
      x-api-path-slug: actionpurchasescheduledinstances-get
      responses:
        200:
          description: OK
      tags:
      - Scheduled Instance
  /?Action=GetHostReservationPurchasePreview:
    get:
      summary: Get Host Reservation Purchase Preview
      description: |-
        Preview a reservation purchase with configurations that match those of your
                    Dedicated Host.
      operationId: gethostreservationpurchasepreview
      x-api-path-slug: actiongethostreservationpurchasepreview-get
      parameters:
      - in: query
        name: AutoPlacement
        description: Specify whether to enable or disable auto-placement
        type: string
      - in: query
        name: HostId.N
        description: The host IDs of the Dedicated Hosts you want to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Host Reservation
  /?Action=PurchaseHostReservation:
    get:
      summary: Purchase Host Reservation
      description: Purchase a reservation with configurations that match those of
        your Dedicated Host.
      operationId: purchasehostreservation
      x-api-path-slug: actionpurchasehostreservation-get
      parameters:
      - in: query
        name: HostId.N
        description: The IDs of the Dedicated Hosts you want to release
        type: string
      responses:
        200:
          description: OK
      tags:
      - Host Reservation