{
  "info": {
    "name": "Azure Relay API Namespaces List",
    "_postman_id": "81129963-2564-4c3f-a3b6-cbe256d2871c",
    "description": "Lists all the available namespaces within the subscription irrespective of the resourceGroups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "namespaces",
      "item": [
        {
          "id": "e55ee722-5cf6-4703-95bd-12ae9e34d015",
          "name": "Namespaces_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Relay/Namespaces"
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
            "description": "Lists all the available namespaces within the subscription irrespective of the resourceGroups"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f9769ec-b1af-440a-ab7e-7317edfb3398"
            }
          ]
        }
      ]
    }
  ]
}