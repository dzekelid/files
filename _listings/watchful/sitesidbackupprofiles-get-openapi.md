---
swagger: "2.0"
x-collection-name: Watchful
x-complete: 0
info:
  title: Watchful Return Backup Profile
  description: Return backup profile
  version: 1.0.0
host: watchful.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sites/{id}/backupprofiles:
    get:
      summary: Return Backup Profile
      description: Return backup profile
      operationId: getBackupProfiles
      x-api-path-slug: sitesidbackupprofiles-get
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Backupprofiles
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