{
  "info": {
    "name": "Azure Relay API Namespaces List By Resource Group",
    "_postman_id": "0a6124dc-a538-4f32-bb67-9dcd63653f32",
    "description": "Lists all the available namespaces within the ResourceGroup.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "namespaces resource group",
      "item": [
        {
          "id": "99ad7e06-3ad8-4187-88b7-112fb2bf69ad",
          "name": "Namespaces_ListByResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Relay/Namespaces"
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
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the available namespaces within the ResourceGroup"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36b03d88-9afd-4329-8f23-01b0e1c3eff4"
            }
          ]
        }
      ]
    }
  ]
}