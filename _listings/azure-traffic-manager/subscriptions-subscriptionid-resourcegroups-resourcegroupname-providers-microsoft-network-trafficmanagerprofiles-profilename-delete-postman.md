{
  "info": {
    "name": "Azure Traffic Manager API Profiles Delete",
    "_postman_id": "616c192b-1d7c-45da-bad4-4eaab8f153f4",
    "description": "Deletes a Traffic Manager profile.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "profiles",
      "item": [
        {
          "id": "c470c19a-366b-4848-866f-ea2bd7eee0ec",
          "name": "Profiles_Delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Traffic Manager profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcfabde9-9c6e-4418-8eca-0747924f713e"
            }
          ]
        }
      ]
    }
  ]
}