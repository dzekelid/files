---
name: moltin
x-slug: moltin
description: The comprehensive eCommerce API infrastructure for any platform. Moltin
  handles data storage and eCommerce logic in the cloud so that you can focus on creating
  great customer experiences.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/moltin-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Files
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/moltin/apis.md
specificationVersion: "0.14"
apis:
- name: Moltin - Update Products <=> Files Relationships
  x-api-slug: v2productsproductidrelationshipsfiles-put
  description: '`File`''s specified in the payload willbe related to the product any
    relatiosnhips to `File`''s **NOT** specified in payload will be removed.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/moltin-logo.png
  humanURL: https://moltin.com
  baseURL: https://api.moltin.com//
  tags: Commerce, Target, Commerce, Stack Network, Retail, Kiosk, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/moltin/v2productsproductidrelationshipsfiles-put-openapi.md
- name: Moltin - Create Products <=> Files Relationships
  x-api-slug: v2productsproductidrelationshipsfiles-post
  description: Here you can add `File`'s to a product. `File`'s specified in the payload
    willbe related to the product.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/moltin-logo.png
  humanURL: https://moltin.com
  baseURL: https://api.moltin.com//
  tags: Commerce, Target, Commerce, Stack Network, Retail, Kiosk, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/moltin/v2productsproductidrelationshipsfiles-post-openapi.md
- name: Moltin - Delete Products <=> Files Relationship
  x-api-slug: v2productsproductidrelationshipsfiles-delete
  description: Here you can delete a relationship between a `Product` and `File`'s.
    Only relationships to `File`'s specified in the payload will be removed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/moltin-logo.png
  humanURL: https://moltin.com
  baseURL: https://api.moltin.com//
  tags: Commerce, Target, Commerce, Stack Network, Retail, Kiosk, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/moltin/v2productsproductidrelationshipsfiles-delete-openapi.md
- name: Moltin - Get all files
  x-api-slug: v2files-get
  description: Get all files.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/moltin-logo.png
  humanURL: https://moltin.com
  baseURL: https://api.moltin.com//
  tags: Commerce, Target, Commerce, Stack Network, Retail, Kiosk, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/moltin/v2files-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://mocklab.api.gallery.streamdata.io
- type: x-api-stack
  url: http://moltin.stack.network
- type: x-base
  url: https://api.molt.in/
- type: x-blog
  url: https://molt.in/blog
- type: x-developer
  url: https://molt.in/developers
- type: x-documentation
  url: https://docs.moltin.com/
- type: x-email
  url: support@molt.in
- type: x-github
  url: https://github.com/moltin
- type: x-postman
  url: https://www.getpostman.com/collections/e9bdcde0ccb5a08640e6
- type: x-pricing
  url: https://moltin.com/pricing
- type: x-twitter
  url: https://twitter.com/moltin
- type: x-website
  url: https://moltin.com
- type: x-website
  url: https://molt.in/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---