{
  "info": {
    "name": "Buffer Get Profiles Schedules Mediatypeextension",
    "_postman_id": "db3ad5e3-b2b1-42c4-954b-dcbd2664f274",
    "description": "Returns details of the posting schedules associated with a social media profile.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Profiles",
      "item": [
        {
          "id": "968e7ab4-8a49-49c7-9ca6-af88f30cfb92",
          "name": "set-the-posting-schedules-for-the-specified-social-media-profile-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/schedules/update:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post Profiles Schedules Update Mediatypeextension"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f6116e7-e641-4467-8645-f96d3f248c0a"
            }
          ]
        },
        {
          "id": "bfebdf76-660f-4d14-bb17-4ef3f1dcb4bf",
          "name": "returns-details-of-the-posting-schedules-associated-with-a-social-media-profile-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/schedules:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns details of the posting schedules associated with a social media profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0b5db51-ee0d-4e09-92af-9dd2283a60ff"
            }
          ]
        }
      ]
    }
  ]
}