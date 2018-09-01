{
  "info": {
    "name": "Taxamo Get Transaction Refunds",
    "_postman_id": "04cbd568-6eb7-4b9f-8fec-d24092c17357",
    "description": "Get transaction refunds.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Detailed",
      "item": [
        {
          "id": "f1e0824b-67f4-432f-aeaa-1f8189509b39",
          "name": "getDetailedRefunds",
          "request": {
            "url": "http://api.taxamo.com/api/v1/settlement/detailed_refunds?country_codes=%7B%7D&date_from=%7B%7D&date_to=%7B%7D&format=%7B%7D&limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detailed refunds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b24e1b90-ad7f-475c-8c27-880d8f2d30c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Fetch",
      "item": [
        {
          "id": "18ca2281-2932-4f59-9c23-05380c637e39",
          "name": "getRefunds",
          "request": {
            "url": "http://api.taxamo.com/api/v1/settlement/refunds?date_from=%7B%7D&format=%7B%7D&moss_country_code=%7B%7D&tax_region=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch refunds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0e8e5b3-1358-4383-ad13-baee9efb10c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Transaction",
      "item": [
        {
          "id": "04bbeddb-0290-4ce4-8e9c-42c0d4bfb0c7",
          "name": "listRefunds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.taxamo.com",
              "path": [
                "api/v1/transactions/:key/refunds"
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
            "description": "Get transaction refunds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfc76159-9107-4a46-93e6-a16053fed14a"
            }
          ]
        }
      ]
    }
  ]
}