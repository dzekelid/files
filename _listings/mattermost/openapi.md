---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost API Reference
  description: -api-v4-is-stable-with-the-mattermost-server-4-0-release--api-v3-was-deprecated-on-january-16th-2018-and-scheduled-for-removal-in-mattermost-v5-0--details-heretagapiv3deprecation--looking-for-the-api-v3-reference-it-has-moved-herehttpsapi-mattermost-comv3-
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{file_id}/thumbnail:
    get:
      summary: Get a files thumbnail
      description: |-
        Gets a file's thumbnail.
        ##### Permissions
        Must have `read_channel` permission or be uploader of the file.
      operationId: gets-a-files-thumbnail-permissionsmust-have-read-channel-permission-or-be-uploader-of-the-file
      x-api-path-slug: filesfile-idthumbnail-get
      parameters:
      - in: path
        name: file_id
        description: The ID of the file to get
      responses:
        200:
          description: OK
      tags:
      - Files
      - Thumbnail
  /files/{file_id}/preview:
    get:
      summary: Get a files preview
      description: |-
        Gets a file's preview.
        ##### Permissions
        Must have `read_channel` permission or be uploader of the file.
      operationId: gets-a-files-preview-permissionsmust-have-read-channel-permission-or-be-uploader-of-the-file
      x-api-path-slug: filesfile-idpreview-get
      parameters:
      - in: path
        name: file_id
        description: The ID of the file to get
      responses:
        200:
          description: OK
      tags:
      - Files
      - Preview
---