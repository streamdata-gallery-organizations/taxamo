{
  "info": {
    "name": "Taxamo Retrieve Transaction Data.",
    "_postman_id": "11539dc9-7baf-4b62-86a9-f4cd0996dc67",
    "description": "Retrieve transaction data..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "823db65e-5a7c-4c12-8803-69830c64dc99",
          "name": "getTransaction",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.taxamo.com",
              "path": [
                "api/v1/transactions/:key"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve transaction data.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ecc2ebb7-6551-4293-8aa3-d0d5c6dfcb63"
            }
          ]
        }
      ]
    }
  ]
}