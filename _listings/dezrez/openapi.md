swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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