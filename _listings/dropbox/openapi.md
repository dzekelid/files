swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox Notify Appendix API v1
  description: the-dropbox-notify--is-a-part-of-dropbox-core-ap-with-a-separate-endpoint-for-notification-call-
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-notify.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{root}/{path}:
    get:
      summary: Downloads a file.
      description: |-
        Downloads a file.

        This method also supports [HTTP Range Retrieval Requests](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.35.2)
        to allow retrieving partial file contents.
      operationId: downloads-a-filethis-method-also-supports-http-range-retrieval-requestshttpwwww3orgprotocolsrfc2616r
      x-api-path-slug: filesrootpath-get
      parameters:
      - in: path
        name: path
        description: The path to the file you want to retrieve
      - in: query
        name: rev
        description: The revision of the file to retrieve
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Files
      - Root
      - Path
  /files_put/{root}/{path}:
    post:
      summary: Uploads a file using PUT semantics.
      description: |-
        Uploads a file using PUT semantics.

        The preferred HTTP method for this call is **PUT**. For compatibility with browser environments, the **POST**
        HTTP method is also recognized.

        **Note:** Providing a `Content-Length` header set to the size of the uploaded file is required so that the
        server can verify that it has received the entire file contents.

        **Note:** `/files_put` has a maximum file size limit of 150 MB and does not support uploads with chunked
        encoding. To upload larger files, use [/chunked_upload](https://www.dropbox.com/developers/core/docs#chunked-upload)
        instead.
      operationId: uploads-a-file-using-put-semanticsthe-preferred-http-method-for-this-call-is-put-for-compatibility-w
      x-api-path-slug: files-putrootpath-post
      parameters:
      - in: query
        name: autorename
        description: This value, either `true` (default) or `false`, determines what
          happens when there is a conflict
      - in: body
        name: file_content
        description: The file contents to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: locale
        description: The metadata returned on successful upload will have its `size`
          field translated based on the given locale
      - in: query
        name: overwrite
        description: This value, either `true` (default) or `false`, determines whether
          an existing file will be overwrittenby this upload
      - in: query
        name: parent_rev
        description: If present, this parameter specifies the revision of the file
          youre editing
      - in: path
        name: path
        description: The full path to the file you want to write to
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Files
      - Put
      - Root
      - Path
    put:
      summary: Uploads a file using PUT semantics.
      description: |-
        Uploads a file using PUT semantics.

        The preferred HTTP method for this call is **PUT**. For compatibility with browser environments, the **POST**
        HTTP method is also recognized.

        **Note:** Providing a `Content-Length` header set to the size of the uploaded file is required so that the
        server can verify that it has received the entire file contents.

        **Note:** `/files_put` has a maximum file size limit of 150 MB and does not support uploads with chunked
        encoding. To upload larger files, use [/chunked_upload](https://www.dropbox.com/developers/core/docs#chunked-upload)
        instead.
      operationId: uploads-a-file-using-put-semanticsthe-preferred-http-method-for-this-call-is-put-for-compatibility-w
      x-api-path-slug: files-putrootpath-put
      parameters:
      - in: query
        name: autorename
        description: This value, either `true` (default) or `false`, determines what
          happens when there is a conflict
      - in: body
        name: file_content
        description: The file contents to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: locale
        description: The metadata returned on successful upload will have its `size`
          field translated based on the given locale
      - in: query
        name: overwrite
        description: This value, either `true` (default) or `false`, determines whether
          an existing file will be overwrittenby this upload
      - in: query
        name: parent_rev
        description: If present, this parameter specifies the revision of the file
          youre editing
      - in: path
        name: path
        description: The full path to the file you want to write to
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Files
      - Put
      - Root
      - Path
  /fileops/copy:
    post:
      summary: Copies a file or folder to a new location.
      description: Copies a file or folder to a new location.
      operationId: copies-a-file-or-folder-to-a-new-location
      x-api-path-slug: fileopscopy-post
      parameters:
      - in: formData
        name: from_copy_ref
        description: Specifies a `copy_ref` generated from a previous [/copy_ref](https://www
      - in: formData
        name: from_path
        description: Specifies the file or folder to be copied from relative to `root`
      - in: formData
        name: locale
        description: The metadata returned will have its `size` field translated based
          on the given locale
      - in: formData
        name: root
        description: The root relative to which `from_path` and `to_path` are specified
      - in: formData
        name: to_path
        description: Specifies the destination path, *including the new name for the
          file or folder*, relative to `root`
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Fileops
      - Copy
  /fileops/create_folder:
    post:
      summary: Create Folder
      description: /fileops/create_folder
      operationId: fileopscreate-folder
      x-api-path-slug: fileopscreate-folder-post
      parameters:
      - in: query
        name: locale
        description: The metadata returned will have its size field translated based
          on the given locale
      - in: query
        name: path
        description: The path to the new folder to create relative to root
      - in: query
        name: root
        description: The root relative to which path is specified
      responses:
        200:
          description: OK
      tags:
      - Fileops
      - Create
      - Folder
  /fileops/delete:
    post:
      summary: Deletes a file or folder.
      description: Deletes a file or folder.
      operationId: deletes-a-file-or-folder
      x-api-path-slug: fileopsdelete-post
      parameters:
      - in: formData
        name: locale
        description: The metadata returned will have its `size` field translated based
          on the given locale
      - in: formData
        name: path
        description: The path to the file or folder to be deleted
      - in: formData
        name: root
        description: The root relative to which `path` is specified
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Fileops
      - Delete
  /fileops/move:
    post:
      summary: Moves a file or folder to a new location.
      description: Moves a file or folder to a new location.
      operationId: moves-a-file-or-folder-to-a-new-location
      x-api-path-slug: fileopsmove-post
      parameters:
      - in: formData
        name: from_path
        description: Specifies the file or folder to be moved from relative to `root`
      - in: formData
        name: locale
        description: The metadata returned will have its `size` field translated based
          on the given locale
      - in: formData
        name: root
        description: The root relative to which `from_path` and `to_path` are specified
      - in: formData
        name: to_path
        description: Specifies the destination path, *including the new name for the
          file or folder*, relative to `root`
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Fileops
      - Move
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