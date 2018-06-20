{
  "info": {
    "name": "Taxamo Locate IP Address",
    "_postman_id": "f30b70f9-cb6f-4bca-972f-7c0c6a8c61dd",
    "description": "Locate ip address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "2e0f024e-8e4d-4d10-bdce-01268dfeadc7",
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
              "id": "3b6d782e-1d0f-43c2-98c4-9be314682d33"
            }
          ]
        }
      ]
    },
    {
      "name": "Currencies",
      "item": [
        {
          "id": "fd6eadb7-51c6-4406-aafc-c6a4da98ada5",
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
              "id": "71475f78-e4ce-48e9-a160-154c62619554"
            }
          ]
        }
      ]
    },
    {
      "name": "Product",
      "item": [
        {
          "id": "12fcc0fd-95e2-4bb6-b612-5c9475fca7e9",
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
              "id": "085dd154-cee5-4c1c-a667-bb8ea67e219e"
            }
          ]
        }
      ]
    },
    {
      "name": "Locate",
      "item": [
        {
          "id": "6f8326c4-857d-4943-bdc4-4c1f088ff765",
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
              "id": "ce91532e-0a9a-4b5b-bf5f-f6ff49f88d0e"
            }
          ]
        }
      ]
    }
  ]
}