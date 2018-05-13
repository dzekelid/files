{
  "info": {
    "name": "Azure Traffic Manager API Profiles List All",
    "_postman_id": "71d2dbe3-b31c-4202-97ca-43ae0aafc3b0",
    "description": "Lists all Traffic Manager profiles within a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "profiles",
      "item": [
        {
          "id": "65dc7714-f907-4e21-bf6e-3515681943ec",
          "name": "Profiles_ListAll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Network/trafficmanagerprofiles"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all Traffic Manager profiles within a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60a649db-44c9-4076-8f93-02fab899b0b8"
            }
          ]
        }
      ]
    }
  ]
}