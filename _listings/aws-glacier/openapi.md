swagger: "2.0"
x-collection-name: AWS Glacier
x-complete: 1
info:
  title: AWS Glacier API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{AccountId}/provisioned-capacity:
    post:
      summary: Purchase  Provisioned  Capacity
      description: |-
        Purchase Provisioned Capacity (POST provisioned-capacity)This operation purchases a provisioned capacity unit for an AWS account.RequestsTo purchase provisioned capacity unit for an AWS account send an HTTP POST
                 request to the provisioned-capacity URI.
      operationId: Purchase Provisioned Capacity (POST provisioned-capacity)
      x-api-path-slug: accountidprovisionedcapacity-post
      parameters:
      - type: string
      responses:
        200:
          description: OK
      tags:
      - Purchase Provisioned Capacity