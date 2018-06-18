---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Groups API List files
  description: List files.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{group_id}/files:
    get:
      summary: List files
      description: List files.
      operationId: list-files
      x-api-path-slug: groupsgroup-idfiles-get
      parameters:
      - in: query
        name: content_types[]
        description: Filter results by content-type
      - in: query
        name: include[]
        description: Array of additional information to include
      - in: query
        name: only[]
        description: Array of information to restrict to
      - in: query
        name: order
        description: The sorting order
      - in: query
        name: search_term
        description: The partial name of the files to match and return
      - in: query
        name: sort
        description: Sort results by this field
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
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