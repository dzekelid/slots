---
swagger: "2.0"
x-collection-name: Bookeo
x-complete: 1
info:
  title: Bookeo
  version: 1.0.0
host: api.bookeo.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /availability/slots:
    get:
      summary: Get information about the availability of products
      description: |-
        Performs a basic search to find available slots and number of seats in each.
         Note that there are two different searches possible, /availability/slots (this endpoint) and /availability/matchingslots .
         The former simply shows the number of available seats for each available slot. The latter takes as input the participant numbers, and shows the slots that are available for those numbers, and an estimate of the price.
         /availability/slots cannot be used for products of type flexibleTime . For those products, use /availability/matchingslots .
      operationId: getAvailabilitySlots
      x-api-path-slug: availabilityslots-get
      parameters:
      - in: query
        name: endTime
        description: the end time to search to
      - in: query
        name: itemsPerPage
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      - in: query
        name: productId
        description: the product id (see /settings/products)
      - in: query
        name: startTime
        description: the start time to search from
      responses:
        200:
          description: OK
      tags:
      - Availability
      - Slots
---