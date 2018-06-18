{
  "info": {
    "name": "Buffer Post Profiles Schedules Update Mediatypeextension",
    "_postman_id": "8ee1460c-1b55-4232-803e-173b482fdf79",
    "description": "Post Profiles Schedules Update Mediatypeextension",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Profiles",
      "item": [
        {
          "id": "72796075-5939-4cdd-bd0f-ffcc7fbf24f1",
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
              "id": "52ee22ac-dffe-461d-a124-ba0c134e164f"
            }
          ]
        }
      ]
    }
  ]
}