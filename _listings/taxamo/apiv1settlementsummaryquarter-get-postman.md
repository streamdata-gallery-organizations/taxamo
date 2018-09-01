{
  "info": {
    "name": "Taxamo Fetch Summary",
    "_postman_id": "898f43a7-d169-4604-811e-c92cdccf5a75",
    "description": "Fetch summary.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "c234480b-e8eb-4591-952a-09adebdc8644",
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
              "id": "19d2e811-e031-4bab-9c2e-872a5252bf6c"
            }
          ]
        }
      ]
    },
    {
      "name": "Currencies",
      "item": [
        {
          "id": "1745f81e-edde-45b1-af1b-79c3e21d1449",
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
              "id": "45abc289-d14c-40b8-8b85-2441a263ca53"
            }
          ]
        }
      ]
    },
    {
      "name": "Product",
      "item": [
        {
          "id": "e981b37b-970b-4e0a-ad66-76618b20cab3",
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
              "id": "a7d63294-3a74-4cfd-8b9e-22e7195b6943"
            }
          ]
        }
      ]
    },
    {
      "name": "Locate",
      "item": [
        {
          "id": "97a578d7-c072-41e0-9ef8-98f352ac4dc7",
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
              "id": "a87c074e-a5e5-4a58-ae76-434ab5fcb61d"
            }
          ]
        },
        {
          "id": "e27b393f-702f-44fa-ac75-f88c2cb3a7bb",
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
              "id": "acca4e0f-d069-4f7b-9446-ece39e3ee4d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Calculate",
      "item": [
        {
          "id": "560c72bc-9170-46b2-90fc-da5318960c94",
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
              "id": "1f2ba814-6969-43de-9600-226c66ea08d9"
            }
          ]
        },
        {
          "id": "1b80cca9-8d43-4b90-a4a7-f3dae03b7026",
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
              "id": "a83ca333-3927-4240-b9fc-ad67a50751e9"
            }
          ]
        }
      ]
    },
    {
      "name": "Detailed",
      "item": [
        {
          "id": "287e7ae1-6448-4040-861b-c038cc0a9ac3",
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
              "id": "2dee12d6-118f-4b8a-96c3-a95fc643853f"
            }
          ]
        }
      ]
    },
    {
      "name": "Fetch",
      "item": [
        {
          "id": "fa2cd0b7-0beb-409f-b021-6cedf0d2f1e0",
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
              "id": "9b379640-f980-4d48-8876-860a587f541a"
            }
          ]
        },
        {
          "id": "469d6db5-ea73-4a3c-9f93-f334145e838a",
          "name": "getSettlementSummary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.taxamo.com",
              "path": [
                "api/v1/settlement/summary/:quarter"
              ],
              "query": [
                {
                  "key": "end_month",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "moss_country_code",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_month",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tax_region",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "quarter",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "376cfc9c-f19f-46d7-965d-10e35e78e514"
            }
          ]
        }
      ]
    }
  ]
}