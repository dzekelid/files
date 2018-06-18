---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Users API
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
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
  /users/{user_id}/files:
    get:
      summary: List files
      description: List files.
      operationId: list-files
      x-api-path-slug: usersuser-idfiles-get
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
      - Users
      - User
      - Id
      - Files
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: usersuser-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Files
  /users/{user_id}/files/id:
    get:
      summary: Get file
      description: Get file.
      operationId: get-file
      x-api-path-slug: usersuser-idfilesid-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional information to include
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Files
      - Id
  /users/{user_id}/files/quota:
    get:
      summary: Get quota information
      description: Get quota information.
      operationId: get-quota-information
      x-api-path-slug: usersuser-idfilesquota-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Files
      - Quota
---