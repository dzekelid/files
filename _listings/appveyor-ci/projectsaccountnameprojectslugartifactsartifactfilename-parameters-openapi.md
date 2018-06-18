---
swagger: "2.0"
x-collection-name: AppVeyor CI
x-complete: 0
info:
  title: App Veyor Parameters Projects Accountname Projectslug Artifacts Artifactfilename
  description: Parameters projects accountname projectslug artifacts artifactfilename.
  termsOfService: https://www.appveyor.com/terms-of-service/
  contact:
    name: AppVeyor Team
    url: https://www.appveyor.com/about/
    email: team@appveyor.com
  version: 0.20170106.0
host: ci.appveyor.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /buildjobs/{jobId}/artifacts/{artifactFileName}:
    get:
      summary: Get Buildjobs Jobid Artifacts Artifactfilename
      description: Get buildjobs jobid artifacts artifactfilename.
      operationId: getBuildjobsJobArtifactsArtifactfilename
      x-api-path-slug: buildjobsjobidartifactsartifactfilename-get
      responses:
        200:
          description: OK
      tags:
      - Builds
      - Jobs
      - ""
      - Artifacts
      - Files
    parameters:
      summary: Parameters Buildjobs Jobid Artifacts Artifactfilename
      description: Parameters buildjobs jobid artifacts artifactfilename.
      operationId: parametersBuildjobsJobArtifactsArtifactfilename
      x-api-path-slug: buildjobsjobidartifactsartifactfilename-parameters
      responses:
        200:
          description: OK
      tags:
      - Builds
      - Jobs
      - ""
      - Artifacts
      - Files
  /projects/{accountName}/{projectSlug}/artifacts/{artifactFileName}:
    get:
      summary: Get Projects Accountname Projectslug Artifacts Artifactfilename
      description: Get projects accountname projectslug artifacts artifactfilename.
      operationId: getProjectsAccountnameProjectslugArtifactsArtifactfilename
      x-api-path-slug: projectsaccountnameprojectslugartifactsartifactfilename-get
      responses:
        200:
          description: OK
      tags:
      - Projects
      - AccountName
      - ProjectSlug
      - Artifacts
      - Files
    parameters:
      summary: Parameters Projects Accountname Projectslug Artifacts Artifactfilename
      description: Parameters projects accountname projectslug artifacts artifactfilename.
      operationId: parametersProjectsAccountnameProjectslugArtifactsArtifactfilename
      x-api-path-slug: projectsaccountnameprojectslugartifactsartifactfilename-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - AccountName
      - ProjectSlug
      - Artifacts
      - Files
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