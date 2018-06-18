---
swagger: "2.0"
x-collection-name: Azure Traffic Manager
x-complete: 0
info:
  title: Azure Traffic Manager API Profiles Check Traffic Manager Relative Dns Name
    Availability
  version: 1.0.0
  description: Checks the availability of a Traffic Manager Relative DNS name.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /providers/Microsoft.Network/checkTrafficManagerNameAvailability:
    post:
      summary: Profiles Check Traffic Manager Relative Dns Name Availability
      description: Checks the availability of a Traffic Manager Relative DNS name.
      operationId: Profiles_CheckTrafficManagerRelativeDnsNameAvailability
      x-api-path-slug: providersmicrosoft-networkchecktrafficmanagernameavailability-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The Traffic Manager name parameters supplied to the CheckTrafficManagerNameAvailability
          operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Profiles Traffic Manager Relative Dns Name Availability
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