---
name: Box
description: Box Inc. (formerly Box.net) is an online file sharing and Cloud content
  management service for enterprise companies. The company has adopted a freemium
  business model, and provides 5 GB of free storage [3] for personal accounts. A mobile
  version of the service is available for Android, BlackBerry, iOS, WebOS, and Windows
  Phone devices. The company is based in Los Altos, California.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/box1200x630.jpg
x-kinRank: "9"
x-alexaRank: ""
tags:
- Storage
- Storage
- Stack Network
- Stack
- Sharing
- Road Map
- Publishing
- Productivity
- Files
- Collaboration
- Backup
created: "2018-03-23"
modified: "2018-03-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/apis.yaml
specificationVersion: "0.14"
apis:
- name: Box
  description: Box Inc
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/box1200x630.jpg
  humanURL: ""
  baseURL: https://api.box.com//2.0
  tags: Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/files-file-id-metadata-scope-template-delete.md
- name: Box Update File Info, Lock and Unlock, Create Shared Link
  description: |-
    Used to update individual or multiple fields in the file object, including renaming the file, changing its description, and creating a shared link for the file. To move a file, change the ID of its parent folder. An optional If-Match header can be included to prevent race conditions.

    To lock and unlock files, you execute a PUT operation on the /files/{file id} endpoint and set or clear the lock properties on the file.

    Used to create a shared link for this particular file. Please see here for more information on the permissions available for shared links. In order to get default shared link status, set it to an empty access level, i.e. {"shared_link": {}}. In order to disable a shared link, send this same type of PUT request with the value of shared_link set to null, i.e. {"shared_link": null}
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/box1200x630.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/box/files-file-id-put.md
x-common:
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
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
- type: x-website
  url: http://box.com
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
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
- type: x-website
  url: http://box.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---