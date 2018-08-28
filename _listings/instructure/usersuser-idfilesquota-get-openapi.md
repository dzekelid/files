---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Users API Get quota information
  description: Get quota information.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/assignments/assignment_id/submissions/{user_id}/comments/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-idcommentsfiles-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Comments
      - Files
  /courses/{course_id}/assignments/assignment_id/submissions/{user_id}/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Files
  /courses/{course_id}/files:
    get:
      summary: List files
      description: List files.
      operationId: list-files
      x-api-path-slug: coursescourse-idfiles-get
      parameters:
      - in: query
        name: content_types[]
        description: Filter results by content-type
      - in: query
        name: include[]
        description: Array of additional information to include
      - in: query
        name: only[]
        description: Array of information to restrict to
      - in: query
        name: order
        description: The sorting order
      - in: query
        name: search_term
        description: The partial name of the files to match and return
      - in: query
        name: sort
        description: Sort results by this field
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Files
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: coursescourse-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Files
  /courses/{course_id}/files/id:
    get:
      summary: Get file
      description: Get file.
      operationId: get-file
      x-api-path-slug: coursescourse-idfilesid-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional information to include
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Files
      - Id
  /courses/{course_id}/files/quota:
    get:
      summary: Get quota information
      description: Get quota information.
      operationId: get-quota-information
      x-api-path-slug: coursescourse-idfilesquota-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Files
      - Quota
  /courses/{course_id}/quizzes/quiz_id/submissions/self/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsselffiles-post
      parameters:
      - in: query
        name: name
        description: The name of the quiz submission file
      - in: query
        name: on_duplicate
        description: How to handle duplicate names
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Self
      - Files
  /groups/{group_id}/files:
    get:
      summary: List files
      description: List files.
      operationId: list-files
      x-api-path-slug: groupsgroup-idfiles-get
      parameters:
      - in: query
        name: content_types[]
        description: Filter results by content-type
      - in: query
        name: include[]
        description: Array of additional information to include
      - in: query
        name: only[]
        description: Array of information to restrict to
      - in: query
        name: order
        description: The sorting order
      - in: query
        name: search_term
        description: The partial name of the files to match and return
      - in: query
        name: sort
        description: Sort results by this field
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: groupsgroup-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
  /groups/{group_id}/files/id:
    get:
      summary: Get file
      description: Get file.
      operationId: get-file
      x-api-path-slug: groupsgroup-idfilesid-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional information to include
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
      - Id
  /groups/{group_id}/files/quota:
    get:
      summary: Get quota information
      description: Get quota information.
      operationId: get-quota-information
      x-api-path-slug: groupsgroup-idfilesquota-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
      - Quota
  /sections/{section_id}/assignments/assignment_id/submissions/{user_id}/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsuser-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Files
  /users/{user_id}/files:
    get:
      summary: List files
      description: List files.
      operationId: list-files
      x-api-path-slug: usersuser-idfiles-get
      parameters:
      - in: query
        name: content_types[]
        description: Filter results by content-type
      - in: query
        name: include[]
        description: Array of additional information to include
      - in: query
        name: only[]
        description: Array of information to restrict to
      - in: query
        name: order
        description: The sorting order
      - in: query
        name: search_term
        description: The partial name of the files to match and return
      - in: query
        name: sort
        description: Sort results by this field
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Files
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: usersuser-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Files
  /users/{user_id}/files/id:
    get:
      summary: Get file
      description: Get file.
      operationId: get-file
      x-api-path-slug: usersuser-idfilesid-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional information to include
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Files
      - Id
  /users/{user_id}/files/quota:
    get:
      summary: Get quota information
      description: Get quota information.
      operationId: get-quota-information
      x-api-path-slug: usersuser-idfilesquota-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Files
      - Quota
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