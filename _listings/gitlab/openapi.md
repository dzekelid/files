swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/repository/files:
    get:
      summary: Get Projects Repository Files
      description: Get projects repository files.
      operationId: getV3ProjectsIdRepositoryFiles
      x-api-path-slug: v3projectsidrepositoryfiles-get
      parameters:
      - in: query
        name: file_path
        description: The path to the file
      - in: path
        name: id
        description: The project ID
      - in: query
        name: ref
        description: The name of branch, tag, or commit
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Files
    post:
      summary: Post Projects Repository Files
      description: Post projects repository files.
      operationId: postV3ProjectsIdRepositoryFiles
      x-api-path-slug: v3projectsidrepositoryfiles-post
      parameters:
      - in: formData
        name: author_email
        description: The email of the author
      - in: formData
        name: author_name
        description: The name of the author
      - in: formData
        name: branch_name
        description: The name of branch
      - in: formData
        name: commit_message
        description: Commit Message
      - in: formData
        name: content
        description: File content
      - in: formData
        name: encoding
        description: File encoding
      - in: formData
        name: file_path
        description: The path to new file
      - in: path
        name: id
        description: The project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Files
    put:
      summary: Put Projects Repository Files
      description: Update existing file in repository
      operationId: putV3ProjectsIdRepositoryFiles
      x-api-path-slug: v3projectsidrepositoryfiles-put
      parameters:
      - in: formData
        name: author_email
        description: The email of the author
      - in: formData
        name: author_name
        description: The name of the author
      - in: formData
        name: branch_name
        description: The name of branch
      - in: formData
        name: commit_message
        description: Commit Message
      - in: formData
        name: content
        description: File content
      - in: formData
        name: encoding
        description: File encoding
      - in: formData
        name: file_path
        description: The path to new file
      - in: path
        name: id
        description: The project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Files
    delete:
      summary: Delete Projects Repository Files
      description: Delete an existing file in repository
      operationId: deleteV3ProjectsIdRepositoryFiles
      x-api-path-slug: v3projectsidrepositoryfiles-delete
      parameters:
      - in: query
        name: author_email
        description: The email of the author
      - in: query
        name: author_name
        description: The name of the author
      - in: query
        name: branch_name
        description: The name of branch
      - in: query
        name: commit_message
        description: Commit Message
      - in: query
        name: file_path
        description: The path to new file
      - in: path
        name: id
        description: The project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Files