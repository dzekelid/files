{
  "info": {
    "name": "Azure Traffic Manager API Profiles List By In Resource Group",
    "_postman_id": "2fb40c24-4e47-4104-9fe9-c0d30e8d5ded",
    "description": "Lists all Traffic Manager profiles within a resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "profiles",
      "item": [
        {
          "id": "4e4f89c3-5a05-43ed-badb-ad9c3b860f22",
          "name": "Profiles_ListByInResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/trafficmanagerprofiles"
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
            "description": "Lists all Traffic Manager profiles within a resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fba8e10-697f-45dc-8996-744e95c5a4b1"
            }
          ]
        }
      ]
    }
  ]
}