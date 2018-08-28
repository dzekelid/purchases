---
swagger: "2.0"
x-collection-name: AWS Glacier
x-complete: 0
info:
  title: Amazon Glacier API Purchase  Provisioned  Capacity
  version: 1.0.0
  description: |-
    Purchase Provisioned Capacity (POST provisioned-capacity)This operation purchases a provisioned capacity unit for an AWS account.RequestsTo purchase provisioned capacity unit for an AWS account send an HTTP POST
             request to the provisioned-capacity URI.
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