---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Get appliance (Extended warranty, purchase insurance ) certificate
    details.
  description: Get appliance (Extended warranty, purchase insurance ) certificate
    details.
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sales/v1/individual/appliance/certificates/{certificate_id}:
    get:
      summary: Get appliance (Extended warranty, purchase insurance ) certificate
        details.
      description: Get appliance (Extended warranty, purchase insurance ) certificate
        details.
      operationId: getSalesV1IndividualApplianceCertificatesCertificate_id
      x-api-path-slug: salesv1individualappliancecertificatescertificate-id-get
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: path
        name: certificate_id
        description: Certificate unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - appliance
      - (Extended
      - warranty
      - ""
      - purchase
      - insurance
      - )
      - certificate
      - details.
  /sales/v1/individual/appliance/certificates:
    post:
      summary: Requests the activation of a certificate either to cover an appliance
        purchased or to extend the warranty period of an appliance purchased. At least
        one product_criteria has to be specified to identify the product to which
        to subscribe. This endpoint
      description: Requests the activation of a certificate either to cover an appliance
        purchased or to extend the warranty period of an appliance purchased. At least
        one product_criteria has to be specified to identify the product to which
        to subscribe. This endpoint
      operationId: postSalesV1IndividualApplianceCertificates
      x-api-path-slug: salesv1individualappliancecertificates-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - the
      - activation
      - ofcertificate
      - either
      - to
      - coverappliance
      - purchasedto
      - extend
      - the
      - warranty
      - period
      - ofappliance
      - purchased.
      - At
      - leastproduct_criteria
      - haAssistance
      - to
      - be
      - specified
      - to
      - identify
      - the
      - product
      - to
      - which
      - to
      - subscribe.
      - ThiAssistance
      - endpoint
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