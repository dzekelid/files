---
name: Buffer
x-slug: buffer
description: Buffer is an intuitive social media management platform trusted by brands,
  businesses, agencies, and individuals to help drive social media results.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/994-buffer.jpg
x-kinRank: "7"
x-alexaRank: "2789"
tags: Files
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/apis.md
specificationVersion: "0.14"
apis:
- name: Buffer Post Profiles Schedules Update Mediatypeextension
  x-api-slug: buffer
  description: Post Profiles Schedules Update Mediatypeextension
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/994-buffer.jpg
  humanURL: http://bufferapp.com
  baseURL: https://api.bufferapp.com//1///profiles/{id}/schedules/update{mediaTypeExtension}
  tags: Profiles,Id,Schedules,UpdatemediaTypeExtension
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidschedulesupdatemediatypeextension-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidschedulesupdatemediatypeextension-post-openapi.md
- name: Buffer Get Profiles Schedules Mediatypeextension
  x-api-slug: buffer
  description: Returns details of the posting schedules associated with a social media
    profile.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/994-buffer.jpg
  humanURL: http://bufferapp.com
  baseURL: https://api.bufferapp.com//1///profiles/{id}/schedules{mediaTypeExtension}
  tags: Profiles,Id,SchedulesmediaTypeExtension
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidschedulesmediatypeextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidschedulesmediatypeextension-get-openapi.md
- name: Buffer Get Profiles Updates Pending Mediatypeextension
  x-api-slug: buffer
  description: Get Profiles Updates Pending Mediatypeextension
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/994-buffer.jpg
  humanURL: http://bufferapp.com
  baseURL: https://api.bufferapp.com//1///profiles/{id}/updates/pending{mediaTypeExtension}
  tags: Profiles,Id,Updates,PendingmediaTypeExtension
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidupdatespendingmediatypeextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidupdatespendingmediatypeextension-get-openapi.md
- name: Buffer Post Profiles Updates Reorder Mediatypeextension
  x-api-slug: buffer
  description: Edit the order at which statuses for the specified social media profile
    will be sent out of the buffer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/994-buffer.jpg
  humanURL: http://bufferapp.com
  baseURL: https://api.bufferapp.com//1///profiles/{id}/updates/reorder{mediaTypeExtension}
  tags: Profiles,Id,Updates,ReordermediaTypeExtension
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidupdatesreordermediatypeextension-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidupdatesreordermediatypeextension-post-openapi.md
- name: Buffer Get Profiles Updates Sent Mediatypeextension
  x-api-slug: buffer
  description: Returns an array of updates that have been sent from the buffer for
    an individual social media profile.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/994-buffer.jpg
  humanURL: http://bufferapp.com
  baseURL: https://api.bufferapp.com//1///profiles/{id}/updates/sent{mediaTypeExtension}
  tags: Profiles,Id,Updates,SentmediaTypeExtension
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidupdatessentmediatypeextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidupdatessentmediatypeextension-get-openapi.md
- name: Buffer Post Profiles Updates Shuffle Mediatypeextension
  x-api-slug: buffer
  description: Randomize the order at which statuses for the specified social media
    profile will be sent out of the buffer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/994-buffer.jpg
  humanURL: http://bufferapp.com
  baseURL: https://api.bufferapp.com//1///profiles/{id}/updates/shuffle{mediaTypeExtension}
  tags: Profiles,Id,Updates,ShufflemediaTypeExtension
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidupdatesshufflemediatypeextension-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidupdatesshufflemediatypeextension-post-openapi.md
- name: Buffer Get Profiles Mediatypeextension
  x-api-slug: buffer
  description: Returns details of the single specified social media profile.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/994-buffer.jpg
  humanURL: http://bufferapp.com
  baseURL: https://api.bufferapp.com//1///profiles/{id}{mediaTypeExtension}
  tags: Profiles,IdmediaTypeExtension
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidmediatypeextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesidmediatypeextension-get-openapi.md
- name: Buffer Get Profiles Mediatypeextension
  x-api-slug: buffer
  description: Returns an array of social media profiles connected to a users account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/994-buffer.jpg
  humanURL: http://bufferapp.com
  baseURL: https://api.bufferapp.com//1///profiles{mediaTypeExtension}
  tags: ProfilesmediaTypeExtension
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesmediatypeextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/profilesmediatypeextension-get-openapi.md
- name: Buffer
  x-api-slug: buffer
  description: Buffer is an intuitive social media management platform trusted by
    brands, businesses, agencies, and individuals to help drive social media results.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/994-buffer.jpg
  humanURL: http://bufferapp.com
  baseURL: https://api.bufferapp.com//1/
  tags: Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/buffer/openapi.md
x-common:
- type: x-base
  url: https://api.bufferapp.com/
- type: x-blog
  url: http://blog.bufferapp.com
- type: x-blog-rss
  url: http://blog.bufferapp.com/feed/
- type: x-github
  url: https://github.com/joelg
- type: x-crunchbase
  url: https://crunchbase.com/organization/buffer
- type: x-crunchbase
  url: http://www.crunchbase.com/company/buffer
- type: x-developer
  url: https://bufferapp.com/developers
- type: x-email
  url: hello@bufferapp.com
- type: x-email
  url: hello@buffer.com
- type: x-email
  url: copyright@buffer.com
- type: x-email
  url: api@bufferapp.com
- type: x-github
  url: https://github.com/bufferapp
- type: x-pricing
  url: https://buffer.com/pricing
- type: x-twitter
  url: https://twitter.com/buffer
- type: x-website
  url: http://bufferapp.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---