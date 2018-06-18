---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack Add File Comments
  description: Add a comment to an existing file.
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files.comments.edit:
    post:
      summary: Edit File Comments
      description: Edit an existing file comment.
      operationId: files_comments_edit
      x-api-path-slug: files-comments-edit-post
      parameters:
      - in: formData
        name: comment
        description: Text of the comment to edit
      - in: formData
        name: file
        description: File containing the comment to edit
      - in: formData
        name: id
        description: The comment to edit
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Files
      - Comments
  /files.upload:
    post:
      summary: Upload File
      description: Uploads or creates a file.
      operationId: files_upload
      x-api-path-slug: files-upload-post
      parameters:
      - in: formData
        name: channels
        description: Comma-separated list of channel names or IDs where the file will
          be shared
      - in: formData
        name: content
        description: File contents via a POST variable
      - in: formData
        name: file
        description: File contents via `multipart/form-data`
      - in: formData
        name: filename
        description: Filename of file
      - in: formData
        name: filetype
        description: A [file type](/types/file#file_types) identifier
      - in: formData
        name: initial_comment
        description: Initial comment to add to file
      - in: formData
        name: title
        description: Title of file
      - in: formData
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Files
  /files.comments.delete:
    post:
      summary: Delete File Comments
      description: Deletes an existing comment on a file.
      operationId: files_comments_delete
      x-api-path-slug: files-comments-delete-post
      parameters:
      - in: formData
        name: file
        description: File to delete a comment from
      - in: formData
        name: id
        description: The comment to delete
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Files
      - Comments
  /files.revokePublicURL:
    post:
      summary: Revoke Public URL
      description: Revokes public/external sharing access for a file
      operationId: files_revokePublicURL
      x-api-path-slug: files-revokepublicurl-post
      parameters:
      - in: formData
        name: file
        description: File to revoke
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Files
  /files.list:
    get:
      summary: List Files
      description: Lists & filters team files.
      operationId: files_list
      x-api-path-slug: files-list-get
      parameters:
      - in: query
        name: channel
        description: Filter files appearing in a specific channel, indicated by its
          ID
      - in: query
        name: count
      - in: query
        name: page
      - in: query
        name: token
        description: Authentication token
      - in: query
        name: ts_from
        description: Filter files created after this timestamp (inclusive)
      - in: query
        name: ts_to
        description: Filter files created before this timestamp (inclusive)
      - in: query
        name: types
        description: Filter files by type:* `all` - All files* `spaces` - Posts* `snippets`
          - Snippets* `images` - Image files* `gdocs` - Google docs* `zips` - Zip
          files* `pdfs` - PDF filesYou can pass multiple values in the types argument,
          like `types=spaces,snippets`
      - in: query
        name: user
        description: Filter files created by a single user
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Files
  /files.delete:
    post:
      summary: Delete File
      description: Deletes a file.
      operationId: files_delete
      x-api-path-slug: files-delete-post
      parameters:
      - in: formData
        name: file
        description: ID of file to delete
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Files
  /files.info:
    get:
      summary: Get File
      description: Gets information about a team file.
      operationId: files_info
      x-api-path-slug: files-info-get
      parameters:
      - in: query
        name: count
      - in: query
        name: file
        description: Specify a file by providing its ID
      - in: query
        name: page
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Files
  /files.sharedPublicURL:
    post:
      summary: Share Public URL
      description: Enables a file for public/external sharing.
      operationId: files_sharedPublicURL
      x-api-path-slug: files-sharedpublicurl-post
      parameters:
      - in: formData
        name: file
        description: File to share
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Files
  /files.comments.add:
    post:
      summary: Add File Comments
      description: Add a comment to an existing file.
      operationId: files_comments_add
      x-api-path-slug: files-comments-add-post
      parameters:
      - in: formData
        name: comment
        description: Text of the comment to add
      - in: formData
        name: file
        description: File to add a comment to
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Files
      - Comments
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