{
  "info": {
    "name": "Buffer Get Profiles Updates Sent Mediatypeextension",
    "_postman_id": "d69dc4eb-d1e4-4d4b-8158-08f8f9d56e76",
    "description": "Returns an array of updates that have been sent from the buffer for an individual social media profile.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Profiles",
      "item": [
        {
          "id": "8286cb6d-9ee5-430c-9502-9a74fee27dcc",
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
              "id": "0c0bc0ac-0444-47a7-b364-b1b0c5907355"
            }
          ]
        },
        {
          "id": "028e9859-25bc-40ea-a3f6-963e319fe4a2",
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
              "id": "1e713d2e-1ee3-4837-82cc-182d74b76931"
            }
          ]
        },
        {
          "id": "e1248d07-b1a8-4f7e-8fc6-962b76a2e281",
          "name": "returns-an-array-of-updates-that-are-currently-in-the-buffer-for-an-individual-social-media-profile-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/updates/pending:mediaTypeExtension"
              ],
              "query": [
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "since",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "utc",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Get Profiles Updates Pending Mediatypeextension"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce590044-58d4-4349-be25-6a8f4063407b"
            }
          ]
        },
        {
          "id": "48ebf643-62f2-4f5d-8c0a-4c34d4157966",
          "name": "edit-the-order-at-which-statuses-for-the-specified-social-media-profile-will-be-sent-out-of-the-buff",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/updates/reorder:mediaTypeExtension"
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
            "description": "Edit the order at which statuses for the specified social media profile will be sent out of the buffer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc81aec2-0388-4a2d-a19b-b2178b33c6dd"
            }
          ]
        },
        {
          "id": "8b36dd61-ed09-4c45-a02c-c40edb89a828",
          "name": "returns-an-array-of-updates-that-have-been-sent-from-the-buffer-for-an-individual-social-media-profi",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/updates/sent:mediaTypeExtension"
              ],
              "query": [
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "since",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "utc",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Returns an array of updates that have been sent from the buffer for an individual social media profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ccd2304-4f63-42e0-9ea5-884c22857e86"
            }
          ]
        }
      ]
    }
  ]
}