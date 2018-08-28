{
  "info": {
    "name": "App Veyor Get Buildjobs Jobid Artifacts Artifactfilename",
    "_postman_id": "810f01b0-4fbb-4f0c-9037-efba26867b16",
    "description": "Get buildjobs jobid artifacts artifactfilename.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Builds",
      "item": [
        {
          "id": "2c9d722b-6ff6-4152-861f-29c19771c0ce",
          "name": "getBuildjobsJobArtifactsArtifactfilename",
          "request": {
            "url": {
              "protocol": "http",
              "host": "ci.appveyor.com",
              "path": [
                "api",
                "buildjobs/:jobId/artifacts/:artifactFileName"
              ],
              "variable": [
                {
                  "id": "jobId",
                  "value": "jobId",
                  "type": "string"
                },
                {
                  "id": "artifactFileName",
                  "value": "artifactFileName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get buildjobs jobid artifacts artifactfilename."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce9c195b-b177-4139-9650-7390691de402"
            }
          ]
        }
      ]
    }
  ]
}