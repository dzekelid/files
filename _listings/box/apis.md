---
name: Box
x-slug: box
description: Box is changing how you manage content across your business from simple
  file sharing to building custom apps.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
x-kinRank: "9"
x-alexaRank: "443"
tags: Files
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/apis.md
specificationVersion: "0.14"
apis:
- name: Box File upload preflight check
  x-api-slug: box
  description: The Pre-flight check API will verify that a file will be accepted by
    Box before you send all the bytes over the wire.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/content
  tags: Documents,Files, Content
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filescontent-options-openapi.md
- name: Box Get File's Info, Get Embed Link
  x-api-slug: box
  description: Used to retrieve the metadata about a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}
  tags: Documents,Files, File
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-id-get-openapi.md
- name: Box Update File Info, Lock and Unlock, Create Shared Link
  x-api-slug: box
  description: |-
    Used to update individual or multiple fields in the file object, including renaming the file, changing its description, and creating a shared link for the file. To move a file, change the ID of its parent folder. An optional If-Match header can be included to prevent race conditions.

    To lock and unlock files, you execute a PUT operation on the /files/{file id} endpoint and set or clear the lock properties on the file.

    Used to create a shared link for this particular file. Please see here for more information on the permissions available for shared links. In order to get default shared link status, set it to an empty access level, i.e. {"shared_link": {}}. In order to disable a shared link, send this same type of PUT request with the value of shared_link set to null, i.e. {"shared_link": null}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}
  tags: Documents,Files, File
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-id-put-openapi.md
- name: Box Delete File
  x-api-slug: box
  description: "Discards a file to the trash. The etag of the file can be included
    as an \u2018If-Match\u2019 header to prevent race conditions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}
  tags: Documents,Files, File
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-id-delete-openapi.md
- name: Box Restore Item
  x-api-slug: box
  description: Restores an item that has been moved to the trash. Default behavior
    is to restore the item to the folder it was in before it was moved to the trash.
    If that parent folder no longer exists or if there is now an item with the same
    name in that parent folder, the new parent folder and/or new name will need to
    be included in the request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}
  tags: Documents,Files, File
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-id-post-openapi.md
- name: Box Download File
  x-api-slug: box
  description: Retrieves the actual data of the file. An optional version parameter
    can be set to download a previous version of the file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/content
  tags: Documents,Files, File, , Content
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idcontent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idcontent-get-openapi.md
- name: Box View Versions
  x-api-slug: box
  description: If there are previous versions of this file, this method can be used
    to retrieve information about the older versions. (Versions are only tracked for
    Box users with premium accounts.)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/versions
  tags: Documents,Files, File, , Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idversions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idversions-get-openapi.md
- name: Box Promote Version
  x-api-slug: box
  description: If there are previous versions of this file, this method can be used
    to promote one of the older versions to the top of the stack. This actually mints
    a copy of the old version and puts it on the top of the versions stack. The file
    will have the exact same contents, the same SHA1/etag, and the same name as the
    original. Other properties such as comments do not get updated to their former
    values.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/versions/current
  tags: Documents,Files, File, , Versions, Current
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idversionscurrent-post-openapi.md
- name: Box Delete Old Version
  x-api-slug: box
  description: Discards a specific file version to the trash. (Depending on the enterprise
    settings for this user, the item will either be actually deleted from Box or moved
    to the trash.)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/versions/{VERSION_ID}
  tags: Documents,Files, File, , Versions, Version
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idversionsversion-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idversionsversion-id-delete-openapi.md
- name: Box Copy File
  x-api-slug: box
  description: Used to create a copy of a file in another folder. The original version
    of the file will not be altered.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/copy
  tags: Documents,Files, File, , Copy
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idcopy-post-openapi.md
- name: Box Get Thumbnail
  x-api-slug: box
  description: Retrieves a thumbnail, or smaller image representation, of this file.
    Sizes of 32x32,64x64, 128x128, and 256x256 can be returned in the .png format
    and sizes of 32x32, 94x94, 160x160, and 320x320 can be returned in the .jpg format.
    Thumbnails can be generated for the image and video file formats listed here.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/thumbnail.{EXTENSION}
  tags: Documents,Files, File, , Thumbnail., Extension
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idthumbnail-extension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idthumbnail-extension-get-openapi.md
- name: Box Get Trashed File
  x-api-slug: box
  description: Retrieves an item that has been moved to the trash.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/trash
  tags: Documents,Files, File, , Trash
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idtrash-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idtrash-get-openapi.md
- name: Box Permanently Delete
  x-api-slug: box
  description: Permanently deletes an item that is in the trash. The item will no
    longer exist in Box. This action cannot be undone.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/trash
  tags: Documents,Files, File, , Trash
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idtrash-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idtrash-delete-openapi.md
- name: Box Get File's Comments
  x-api-slug: box
  description: Retrieves the comments on a particular file, if any exist.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/comments
  tags: Documents,Files, File, , Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idcomments-get-openapi.md
- name: Box Get File's Collaborations
  x-api-slug: box
  description: Use this to get a list of all the collaborations on a file
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/collaborations
  tags: Documents,Files, File, , Collaborations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idcollaborations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idcollaborations-get-openapi.md
- name: Box Get File's Tasks
  x-api-slug: box
  description: Retrieves all of the tasks for given file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/tasks
  tags: Documents,Files, File, , Tasks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idtasks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idtasks-get-openapi.md
- name: Box Get Watermark on File
  x-api-slug: box
  description: Used to retrieve the watermark for a corresponding Box file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/watermark
  tags: Documents,Files, File, , Watermark
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idwatermark-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idwatermark-get-openapi.md
- name: Box Apply Watermark on File
  x-api-slug: box
  description: Used to apply or update the watermark for a corresponding Box file.
    The endpoint accepts a JSON body describing the watermark to apply.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/watermark
  tags: Documents,Files, File, , Watermark
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idwatermark-put-openapi.md
- name: Box Remove Watermark on File
  x-api-slug: box
  description: Used to remove the watermark for a corresponding Box file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/watermark
  tags: Documents,Files, File, , Watermark
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idwatermark-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idwatermark-delete-openapi.md
- name: Box Get all Metadata on File
  x-api-slug: box
  description: Used to retrieve all metadata associated with a given file
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/metadata
  tags: Documents,Files, File, , Metadata
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idmetadata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idmetadata-get-openapi.md
- name: Box Create Metadata on File
  x-api-slug: box
  description: Used to create the metadata template instance for a corresponding Box
    file. When creating metadata, only values that adhere to the metadata template
    schema will be accepted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/metadata/{SCOPE}/{TEMPLATE}
  tags: Documents,Files, File, , Metadata, Scope, Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idmetadatascopetemplate-post-openapi.md
- name: Box Get Metadata on File
  x-api-slug: box
  description: Used to retrieve the metadata template instance for a corresponding
    Box file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/metadata/{SCOPE}/{TEMPLATE}
  tags: Documents,Files, File, , Metadata, Scope, Template
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idmetadatascopetemplate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idmetadatascopetemplate-get-openapi.md
- name: Box Update Metadata on File
  x-api-slug: box
  description: |-
    Used to update the template instance. The request body must follow the JSON-Patch specification, which is represented as a JSON array of operation objects (see examples for more details). Updates can be either add, replace, remove , test, move, or copy. The template instance can only be updated if the template instance already exists. When editing metadata, only values that adhere to the metadata template schema will be accepted.
    The update is applied atomically. If any errors occur during the application of the update operations, the metadata instance remains unchanged.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/metadata/{SCOPE}/{TEMPLATE}
  tags: Documents,Files, File, , Metadata, Scope, Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idmetadatascopetemplate-put-openapi.md
- name: Box Delete Metadata on File
  x-api-slug: box
  description: Used to delete the template instance. To delete custom key:value pairs
    within a template instance, you should refer to the updating metadata section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/metadata/{SCOPE}/{TEMPLATE}
  tags: Documents,Files, File, , Metadata, Scope, Template
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idmetadatascopetemplate-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/filesfile-idmetadatascopetemplate-delete-openapi.md
- name: Box
  x-api-slug: box
  description: Box.net provides a sophisticated API for their online document sharing
    and collaboration web application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/openapi.md
x-common:
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
- type: x-crunchbase
  url: https://crunchbase.com/organization/box
- type: x-developer
  url: http://developers.box.com
- type: x-github
  url: https://github.com/boxdotnet
- type: x-pricing
  url: https://developers.box.com/box-platform-pricing/
- type: x-road-map
  url: https://developers.box.com/roadmap/
- type: x-twitter
  url: https://twitter.com/BoxPlatform
- type: x-twitter
  url: https://twitter.com/BoxHQ
- type: x-website
  url: http://box.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---