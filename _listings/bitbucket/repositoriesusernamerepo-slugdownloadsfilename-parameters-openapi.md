---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Repositories Username Repo Slug Downloads Filename
  description: Parameters repositories username repo slug downloads filename
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /snippets/{username}/{encoded_id}/{node_id}/files/{path}:
    get:
      summary: Get Snippets Username Encoded  Node  Files Path
      description: |-
        Retrieves the raw contents of a specific file in the snippet. The
        `Content-Disposition` header will be "attachment" to avoid issues with
        malevolent executable files.

        The file's mime type is derived from its filename and returned in the
        `Content-Type` header.

        Note that for text files, no character encoding is included as part of
        the content type.
      operationId: getSnippetsUsernameEncodedNodeFilesPath
      x-api-path-slug: snippetsusernameencoded-idnode-idfilespath-get
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Node
      - ""
      - Files
      - Path
    parameters:
      summary: Parameters Snippets Username Encoded  Node  Files Path
      description: Parameters snippets username encoded  node  files path
      operationId: parametersSnippetsUsernameEncodedNodeFilesPath
      x-api-path-slug: snippetsusernameencoded-idnode-idfilespath-parameters
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Node
      - ""
      - Files
      - Path
  /repositories/{username}/{repo_slug}/downloads/{filename}:
    delete:
      summary: Delete Repositories Username Repo Slug Downloads Filename
      description: Deletes the specified download artifact from the repository.
      operationId: deleteRepositoriesUsernameRepoSlugDownloadsFilename
      x-api-path-slug: repositoriesusernamerepo-slugdownloadsfilename-delete
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Downloads
      - Filename
    get:
      summary: Get Repositories Username Repo Slug Downloads Filename
      description: |-
        Return a redirect to the contents of a download artifact.

        This endpoint returns the actual file contents and not the artifact's
        metadata.

            $ curl -s -L https://api.bitbucket.org/2.0/repositories/evzijst/git-tests/downloads/hello.txt
            Hello World
      operationId: getRepositoriesUsernameRepoSlugDownloadsFilename
      x-api-path-slug: repositoriesusernamerepo-slugdownloadsfilename-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Downloads
      - Filename
    parameters:
      summary: Parameters Repositories Username Repo Slug Downloads Filename
      description: Parameters repositories username repo slug downloads filename
      operationId: parametersRepositoriesUsernameRepoSlugDownloadsFilename
      x-api-path-slug: repositoriesusernamerepo-slugdownloadsfilename-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Downloads
      - Filename
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