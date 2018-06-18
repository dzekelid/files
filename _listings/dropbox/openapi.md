---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox
  description: the-dropbox-api-allows-you-to-build-the-power-of-dropbox-directly-into-your-app-
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
---