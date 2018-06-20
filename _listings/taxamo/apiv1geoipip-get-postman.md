{
  "info": {
    "name": "Taxamo Locate Provided IP Address",
    "_postman_id": "2fbeb1ba-62a6-4701-8fa3-1ede2a5613f3",
    "description": "Locate provided ip address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "1dfa9c52-4c51-440f-81b4-76de08ddfacb",
          "name": "getCountriesDict",
          "request": {
            "url": "http://api.taxamo.com/api/v1/dictionaries/countries?tax_supported=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Countries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "206dc1fb-dc88-4ae0-bc68-99f7c0fb934c"
            }
          ]
        }
      ]
    },
    {
      "name": "Currencies",
      "item": [
        {
          "id": "03a5da72-8a03-4a6d-b9a5-a71f3d66b67e",
          "name": "getCurrenciesDict",
          "request": {
            "url": "http://api.taxamo.com/api/v1/dictionaries/currencies",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Currencies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c80902e-8efd-4dfa-a299-44aacddf4fc0"
            }
          ]
        }
      ]
    },
    {
      "name": "Product",
      "item": [
        {
          "id": "a0c7d182-3ed5-4072-8ff0-224b15a80aec",
          "name": "getProductTypesDict",
          "request": {
            "url": "http://api.taxamo.com/api/v1/dictionaries/product_types",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Product types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21945973-d342-4b9b-a8b2-697e4706c91c"
            }
          ]
        }
      ]
    },
    {
      "name": "Locate",
      "item": [
        {
          "id": "ea7618f1-b637-4a7e-8cb0-daa41b6d50c6",
          "name": "locateMyIP",
          "request": {
            "url": "http://api.taxamo.com/api/v1/geoip",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Locate ip address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98f3401a-2a62-4d3d-9bdf-00f2b50d56b9"
            }
          ]
        },
        {
          "id": "adb53d35-b036-4ae0-94b8-2861077969e5",
          "name": "locateGivenIP",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.taxamo.com",
              "path": [
                "api/v1/geoip/:ip"
              ],
              "variable": [
                {
                  "id": "ip",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Locate provided ip address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "864d7b4e-dec4-4379-bd3d-0d273118bc1e"
            }
          ]
        }
      ]
    }
  ]
}