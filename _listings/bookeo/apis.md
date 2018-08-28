---
name: Bookeo
x-slug: bookeo
description: Bookeo provides a leading online booking and scheduling system for tours,
  classes, and appointments, to help you save money and time. Click to learn more!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
x-kinRank: "7"
x-alexaRank: "23042"
tags: Slots
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/slots/master/_listings/bookeo/apis.md
specificationVersion: "0.14"
apis:
- name: Bookeo - Get information about the availability of products
  x-api-slug: availabilityslots-get
  description: |-
    Performs a basic search to find available slots and number of seats in each.
     Note that there are two different searches possible, /availability/slots (this endpoint) and /availability/matchingslots .
     The former simply shows the number of available seats for each available slot. The latter takes as input the participant numbers, and shows the slots that are available for those numbers, and an estimate of the price.
     /availability/slots cannot be used for products of type flexibleTime . For those products, use /availability/matchingslots .
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slots/master/_listings/bookeo/availabilityslots-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://bmc.software.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bookeo.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bookeo
- type: x-developer
  url: https://www.bookeo.com/api/
- type: x-documentation
  url: https://www.bookeo.com/apiref/index.html
- type: x-partners
  url: https://www.bookeo.com/affiliate/
- type: x-privacy-policy
  url: https://www.bookeo.com/privacy/
- type: x-terms-of-service
  url: https://www.bookeo.com/termsofservice/
- type: x-twitter
  url: https://twitter.com/bookeo
- type: x-webhook
  url: https://www.bookeo.com/api/webhooks/
- type: x-website
  url: https://www.bookeo.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---