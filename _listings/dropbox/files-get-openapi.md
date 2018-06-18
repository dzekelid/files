---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Dropbox Datastore API Get File
  description: /files (GET)
  version: "1"
host: api.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files:
    get:
      summary: Get File
      description: /files (GET)
      operationId: files-get
      x-api-path-slug: files-get
      parameters:
      - in: query
        name: path
        description: The path to the file you want to retrieve
      - in: query
        name: rev
        description: The revision of the file to retrieve
      responses:
        200:
          description: OK
      tags:
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