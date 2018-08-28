swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /flow-templates/{flowTemplateId}/flows/{flowId}/config/{fileName}:
    get:
      summary: Get Flow Templates Flowtemplateid Flows Flowid Config Filename
      description: Get flow templates flowtemplateid flows flowid config filename.
      operationId: getFlowConfigFileUsingGET_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidconfigfilename-get
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Config
      - Filename
    delete:
      summary: Delete Flow Templates Flowtemplateid Flows Flowid Config Filename
      description: Delete flow templates flowtemplateid flows flowid config filename.
      operationId: deleteFlowConfigFileUsingDELETE_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidconfigfilename-delete
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Config
      - Filename
  /flows/{flowId}/config/{fileName}:
    get:
      summary: Get Flows Flowid Config Filename
      description: Get flows flowid config filename.
      operationId: getFlowConfigFileUsingGET
      x-api-path-slug: flowsflowidconfigfilename-get
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Config
      - Filename
    delete:
      summary: Delete Flows Flowid Config Filename
      description: Delete flows flowid config filename.
      operationId: deleteFlowConfigFileUsingDELETE
      x-api-path-slug: flowsflowidconfigfilename-delete
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Config
      - Filename
  /instances/{instanceId}/config/{fileName}:
    get:
      summary: Get Instances Instanceid Config Filename
      description: Get instances instanceid config filename.
      operationId: getInstanceConfigFileUsingGET
      x-api-path-slug: instancesinstanceidconfigfilename-get
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Config
      - Filename