---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Set the estimated completion date on a purchasing role
  version: 1.0.0
  description: Set the estimated completion date on a purchasing role.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/progression/addprogressionnote:
    post:
      summary: Add a note to a purchasing role
      description: Add a note to a purchasing role.
      operationId: Progression_AddProgressionNoteByprogressionNoteCommandDataContract
      x-api-path-slug: apiprogressionaddprogressionnote-post
      parameters:
      - in: body
        name: progressionNoteCommandDataContract
        description: Details of the progression note
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Note
      - To
      - Purchasing
      - Role
  /api/progression/sales/setestimatedcompletiondate:
    put:
      summary: Set the estimated completion date on a purchasing role
      description: Set the estimated completion date on a purchasing role.
      operationId: SalesProgression_SetEstimatedCompletionDateByprogressionDateCommandDataContract
      x-api-path-slug: apiprogressionsalessetestimatedcompletiondate-put
      parameters:
      - in: body
        name: progressionDateCommandDataContract
        description: The id and datetime of the purchasing role to update the estimated
          completion date for
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Estimated
      - Completion
      - Date
      - "On"
      - Purchasing
      - Role
  /api/progression/sales/setestimatedexchangedate:
    put:
      summary: Set the estimated exchange date on a purchasing role
      description: Set the estimated exchange date on a purchasing role.
      operationId: SalesProgression_SetEstimatedExchangeDateByprogressionDateCommandDataContract
      x-api-path-slug: apiprogressionsalessetestimatedexchangedate-put
      parameters:
      - in: body
        name: progressionDateCommandDataContract
        description: The id and datetime of the purchasing role to update the estimated
          exchange date for
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Estimated
      - Exchange
      - Date
      - "On"
      - Purchasing
      - Role
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