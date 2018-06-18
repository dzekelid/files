---
name: Dropbox
x-slug: dropbox
description: Dropbox is a modern workspace designed to reduce busywork-so you can
  focus on the things that matter. Sign in and put your creative energy to work.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/184-dropbox.jpg
x-kinRank: "10"
x-alexaRank: "89"
tags: Files
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/dropbox/apis.md
specificationVersion: "0.14"
apis:
- name: Dropbox Content Downloads a file.
  x-api-slug: dropbox-content
  description: |-
    Downloads a file.

    This method also supports [HTTP Range Retrieval Requests](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.35.2)
    to allow retrieving partial file contents.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/184-dropbox.jpg
  humanURL: http://dropbox.com
  baseURL: https://api-content.dropbox.com//1//files/{root}/{path}
  tags: Storage,Documents,Files,Root,Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/dropbox/filesrootpath-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/dropbox/filesrootpath-get-openapi.md
- name: Dropbox Content Uploads a file using PUT semantics.
  x-api-slug: dropbox-content
  description: |-
    Uploads a file using PUT semantics.

    The preferred HTTP method for this call is **PUT**. For compatibility with browser environments, the **POST**
    HTTP method is also recognized.

    **Note:** Providing a `Content-Length` header set to the size of the uploaded file is required so that the
    server can verify that it has received the entire file contents.

    **Note:** `/files_put` has a maximum file size limit of 150 MB and does not support uploads with chunked
    encoding. To upload larger files, use [/chunked_upload](https://www.dropbox.com/developers/core/docs#chunked-upload)
    instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/184-dropbox.jpg
  humanURL: http://dropbox.com
  baseURL: https://api-content.dropbox.com//1//files_put/{root}/{path}
  tags: Storage,Documents,Files,Put,Root,Path
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/dropbox/files-putrootpath-post-openapi.md
- name: Dropbox Content Uploads a file using PUT semantics.
  x-api-slug: dropbox-content
  description: |-
    Uploads a file using PUT semantics.

    The preferred HTTP method for this call is **PUT**. For compatibility with browser environments, the **POST**
    HTTP method is also recognized.

    **Note:** Providing a `Content-Length` header set to the size of the uploaded file is required so that the
    server can verify that it has received the entire file contents.

    **Note:** `/files_put` has a maximum file size limit of 150 MB and does not support uploads with chunked
    encoding. To upload larger files, use [/chunked_upload](https://www.dropbox.com/developers/core/docs#chunked-upload)
    instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/184-dropbox.jpg
  humanURL: http://dropbox.com
  baseURL: https://api-content.dropbox.com//1//files_put/{root}/{path}
  tags: Storage,Documents,Files,Put,Root,Path
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/dropbox/files-putrootpath-put-openapi.md
- name: Dropbox Content
  x-api-slug: dropbox-content
  description: Dropbox is a modern workspace designed to reduce busywork-so you can
    focus on the things that matter. Sign in and put your creative energy to work.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/184-dropbox.jpg
  humanURL: http://dropbox.com
  baseURL: https://api-content.dropbox.com//1
  tags: Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/dropbox/openapi.md
- name: Dropbox Datastore API Get File
  x-api-slug: dropbox-datastore-api
  description: /files (GET)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/184-dropbox.jpg
  humanURL: http://dropbox.com
  baseURL: https://api.dropbox.com//1//files
  tags: Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/dropbox/files-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/dropbox/files-get-openapi.md
- name: Dropbox Datastore API
  x-api-slug: dropbox-datastore-api
  description: Keep your apps structured data in sync with Dropbox
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/184-dropbox.jpg
  humanURL: http://dropbox.com
  baseURL: https://api.dropbox.com//1
  tags: Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/dropbox/openapi.md
x-common:
- type: x-application-management
  url: https://www.dropbox.com/developers/apps
- type: x-base
  url: https://api.dropbox.com/
- type: x-blog
  url: https://blog.dropbox.com/
- type: x-blog-rss
  url: https://blog.dropbox.com/feed/
- type: x-branding
  url: https://www.dropbox.com/developers/reference/branding
- type: x-branding
  url: https://www.dropbox.com/branding
- type: x-contact-form
  url: https://www.dropbox.com/developers/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/dropbox
- type: x-crunchbase
  url: https://crunchbase.com/organization/dropbox
- type: x-developer
  url: https://www.dropbox.com/developers
- type: x-email
  url: privacyshield@dropbox.com
- type: x-email
  url: privacy@dropbox.com
- type: x-email
  url: contractnotices@dropbox.com
- type: x-email
  url: copyright@dropbox.com
- type: x-email
  url: dispute-notice@dropbox.com
- type: x-faq
  url: https://www.dropbox.com/developers/support
- type: x-forum
  url: https://www.dropboxforum.com/hc/communities/public/topics/200209245-API-Development
- type: x-github
  url: https://github.com/dropbox
- type: x-pricing
  url: https://www.dropbox.com/plans
- type: x-privacy
  url: https://www.dropbox.com/privacy
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/dropbox-api?sort=votes&pagesize=15
- type: x-support
  url: https://www.dropbox.com/help
- type: x-terms-of-service
  url: https://www.dropbox.com/privacy#terms
- type: x-transparency-report
  url: https://www.dropbox.com/transparency
- type: x-twitter
  url: https://twitter.com/dropbox
- type: x-webhooks
  url: https://www.dropbox.com/developers/webhooks/docs
- type: x-website
  url: http://dropbox.com
- type: x-website
  url: https://www.dropbox.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---