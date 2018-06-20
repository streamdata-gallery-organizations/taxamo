{
  "info": {
    "name": "Taxamo Calculate EU VIES Report",
    "_postman_id": "5d80c00b-d23f-4661-8b42-aae2af4fee26",
    "description": "Calculate eu vies report.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "f46ac705-e2ef-4ce5-82f0-f5310bf2e491",
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
              "id": "d025f761-68f5-4f02-a330-a325935041e9"
            }
          ]
        }
      ]
    },
    {
      "name": "Currencies",
      "item": [
        {
          "id": "1c707f03-db21-4431-8ee5-f80b4b953f96",
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
              "id": "3cb87cad-46bd-4842-876f-65f61da80a7a"
            }
          ]
        }
      ]
    },
    {
      "name": "Product",
      "item": [
        {
          "id": "a99ff418-b984-4244-8605-5343d0586521",
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
              "id": "0af0aafe-4b06-4a1b-8354-8512499b7041"
            }
          ]
        }
      ]
    },
    {
      "name": "Locate",
      "item": [
        {
          "id": "2dea3e2b-cb2a-4c8b-adf3-906e5e82a4fa",
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
              "id": "f59355bd-0ad8-4aad-b6f9-2d6617346291"
            }
          ]
        },
        {
          "id": "039065c6-aa67-4496-ace4-54f7623f2dc1",
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
              "id": "178f6fd7-25a6-4e5a-a249-1363115b014d"
            }
          ]
        }
      ]
    },
    {
      "name": "Calculate",
      "item": [
        {
          "id": "3cdd7ade-2a97-40fd-999e-76b55c65c1ad",
          "name": "getDomesticSummaryReport",
          "request": {
            "url": "http://api.taxamo.com/api/v1/reports/domestic/summary?country_code=%7B%7D&currency_code=%7B%7D&end_month=%7B%7D&format=%7B%7D&fx_date_type=%7B%7D&start_month=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Calculate domestic summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "756ab439-08cc-4278-9a04-b0c0f32d40b6"
            }
          ]
        },
        {
          "id": "c24b8711-ec67-4bdd-8be2-905c557ddd1b",
          "name": "getEuViesReport",
          "request": {
            "url": "http://api.taxamo.com/api/v1/reports/eu/vies?currency_code=%7B%7D&end_month=%7B%7D&eu_country_code=%7B%7D&format=%7B%7D&fx_date_type=%7B%7D&lff_sequence_number=%7B%7D&period_length=%7B%7D&start_month=%7B%7D&tax_id=%7B%7D&transformation=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Calculate eu vies report."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5d81146-d6c6-4b18-afb9-dc2a19efda6a"
            }
          ]
        }
      ]
    }
  ]
}