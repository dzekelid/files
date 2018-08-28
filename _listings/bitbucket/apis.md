---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Files
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket - Get Snippets Username Encoded  Node  Files Path
  x-api-slug: snippetsusernameencoded-idnode-idfilespath-get
  description: |-
    Retrieves the raw contents of a specific file in the snippet. The
    `Content-Disposition` header will be "attachment" to avoid issues with
    malevolent executable files.

    The file's mime type is derived from its filename and returned in the
    `Content-Type` header.

    Note that for text files, no character encoding is included as part of
    the content type.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/snippetsusernameencoded-idnode-idfilespath-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/snippetsusernameencoded-idnode-idfilespath-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Node  Files Path
  x-api-slug: snippetsusernameencoded-idnode-idfilespath-parameters
  description: Parameters snippets username encoded  node  files path
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/snippetsusernameencoded-idnode-idfilespath-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/snippetsusernameencoded-idnode-idfilespath-parameters-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-delete
  description: Deletes the specified download artifact from the repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-get
  description: |-
    Return a redirect to the contents of a download artifact.

    This endpoint returns the actual file contents and not the artifact's
    metadata.

        $ curl -s -L https://api.bitbucket.org/2.0/repositories/evzijst/git-tests/downloads/hello.txt
        Hello World
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-parameters
  description: Parameters repositories username repo slug downloads filename
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-parameters-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-delete
  description: Deletes the specified download artifact from the repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-get
  description: |-
    Return a redirect to the contents of a download artifact.

    This endpoint returns the actual file contents and not the artifact's
    metadata.

        $ curl -s -L https://api.bitbucket.org/2.0/repositories/evzijst/git-tests/downloads/hello.txt
        Hello World
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-parameters
  description: Parameters repositories username repo slug downloads filename
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-parameters-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-parameters
  description: Parameters repositories username repo slug downloads filename
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-get
  description: |-
    Return a redirect to the contents of a download artifact.

    This endpoint returns the actual file contents and not the artifact's
    metadata.

        $ curl -s -L https://api.bitbucket.org/2.0/repositories/evzijst/git-tests/downloads/hello.txt
        Hello World
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-get-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-delete
  description: Deletes the specified download artifact from the repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-delete-openapi.md
x-common:
- type: x-api-gallery
  url: http://bigoven.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bitbucket.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---