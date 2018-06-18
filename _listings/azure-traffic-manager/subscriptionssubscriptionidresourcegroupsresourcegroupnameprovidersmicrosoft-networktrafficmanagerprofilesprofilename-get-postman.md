{
  "info": {
    "name": "Azure Traffic Manager API Profiles Get",
    "_postman_id": "f3ed4255-70da-4177-b952-f5f576624c51",
    "description": "Gets a Traffic Manager profile.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "profiles",
      "item": [
        {
          "id": "94d1606c-a245-4953-86d5-910a99287747",
          "name": "Profiles_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/trafficmanagerprofiles/:profileName"
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
                  "id": "profileName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Gets a Traffic Manager profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9a1f32c-e4a3-4ffa-95c2-209a28da77de"
            }
          ]
        }
      ]
    }
  ]
}