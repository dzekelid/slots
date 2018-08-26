---
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
  /api/appointment/suggest:
    post:
      summary: Auto-picks attendees and the next available appointment slot given
        the parameters in the request.
      description: Auto-picks attendees and the next available appointment slot given
        the parameters in the request..
      operationId: Appointment_SuggestAppointmentSlotByrequest
      x-api-path-slug: apiappointmentsuggest-post
      parameters:
      - in: body
        name: request
        description: An appointment suggest request containing information about the
          desired appointment
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Auto-picks
      - Attendees
      - Next
      - Available
      - Appointment
      - Slot
      - Given
      - Parameters
      - In
      - Request
  /api/role/{id}/documentfromplaceholder:
    get:
      summary: Get a single DocumentPlaceholder which is the 'slot' the particular
        document of type+source exists within.
      description: Get a single documentplaceholder which is the 'slot' the particular
        document of type+source exists within..
      operationId: Role_DocumentFromPlaceholderByidByplaceholderTypeByplaceholderSourceTypeBygroupId
      x-api-path-slug: apiroleiddocumentfromplaceholder-get
      parameters:
      - in: query
        name: groupId
        description: Optional group id to filter placeholder for a specific group
          relating to this role
      - in: path
        name: id
        description: Role id
      - in: query
        name: placeholderSourceType
        description: Where did the document come from to fit into the placeholder
          slot
      - in: query
        name: placeholderType
        description: Which type of document placeholder slot is this
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Single
      - DocumentPlaceholder
      - Which
      - Is
      - Slot
      - Particular
      - Document
      - Of
      - Type+source
      - Exists
      - Within
  /api/viewing/{id}/recordslotapproval/{viewingSlotId}:
    put:
      summary: Set approval status of viewing slot on multi viewing appointment
      description: Set approval status of viewing slot on multi viewing appointment.
      operationId: Viewing_RecordViewingSlotApprovalByidByviewingSlotIdBystatus
      x-api-path-slug: apiviewingidrecordslotapprovalviewingslotid-put
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: status
      - in: path
        name: viewingSlotId
      responses:
        200:
          description: OK
      tags:
      - Set
      - Approval
      - Status
      - Of
      - Viewing
      - Slot
      - "On"
      - Multi
      - Viewing
      - Appointment
---