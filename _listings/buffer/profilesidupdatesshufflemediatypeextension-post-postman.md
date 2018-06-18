{
  "info": {
    "name": "Buffer Post Profiles Updates Shuffle Mediatypeextension",
    "_postman_id": "9a1952de-67bf-4e1b-aa87-8d67b80e1562",
    "description": "Randomize the order at which statuses for the specified social media profile will be sent out of the buffer.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Profiles",
      "item": [
        {
          "id": "c0b7ef04-d146-4b90-bf21-fda8237b0f96",
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
              "id": "b61d2947-2107-4b07-9f54-12c2c267b59b"
            }
          ]
        },
        {
          "id": "1032565c-13c5-43b3-83a6-7fe00e898fbf",
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
              "id": "1af668a3-1767-4162-a23c-8cf9616747e0"
            }
          ]
        },
        {
          "id": "41d36155-ec53-44b4-9a37-d440618de87f",
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
              "id": "f4c03442-c87d-4ab8-abc1-a52df73dab94"
            }
          ]
        },
        {
          "id": "60e7aaa0-041e-4815-b06e-244707673867",
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
              "id": "356825b2-a546-4a32-ba59-16324db790c7"
            }
          ]
        },
        {
          "id": "275f608f-043e-4dfe-a568-7bec77970a42",
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
              "id": "47bc97ac-8a84-4447-84b2-b02eed795b84"
            }
          ]
        },
        {
          "id": "0fba4e36-847b-4794-a671-31e2e82d859e",
          "name": "randomize-the-order-at-which-statuses-for-the-specified-social-media-profile-will-be-sent-out-of-the",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "profiles/:id/updates/shuffle:mediaTypeExtension"
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
            "description": "Randomize the order at which statuses for the specified social media profile will be sent out of the buffer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc7e5544-3530-4579-b118-d8e0bb76ade4"
            }
          ]
        }
      ]
    }
  ]
}