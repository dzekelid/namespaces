{
  "info": {
    "name": "Azure Relay API Namespaces Delete",
    "_postman_id": "3f1b27b0-dcfb-4f40-b590-353e71f57ad5",
    "description": "Deletes an existing namespace. This operation also removes all associated resources under the namespace.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "namespaces",
      "item": [
        {
          "id": "f3a7b09c-1c1e-4a09-a217-640cbdd32fe5",
          "name": "Namespaces_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Relay/namespaces/:namespaceName"
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
                },
                {
                  "id": "namespaceName",
                  "value": "namespaceName",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing namespace"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49651a22-83c1-4dfe-8085-6d8d9ee5743f"
            }
          ]
        }
      ]
    }
  ]
}