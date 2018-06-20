{
  "info": {
    "name": "Taxamo Transaction Stats",
    "_postman_id": "a7e6de9e-4a36-4eae-9eb3-a7cfec18988e",
    "description": "Transaction stats.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "b3d653b5-0fc6-48bd-8846-9e92d92fdb55",
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
              "id": "4ef5c3d6-f03b-4453-adc5-73ee5201fd92"
            }
          ]
        }
      ]
    },
    {
      "name": "Currencies",
      "item": [
        {
          "id": "c1bb5737-f33c-4867-9574-e0aa9d77ec67",
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
              "id": "75927801-8f1d-402e-bfef-b13226db0373"
            }
          ]
        }
      ]
    },
    {
      "name": "Product",
      "item": [
        {
          "id": "93d564b5-063e-4429-8451-ead9890c1130",
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
              "id": "ce748ebc-132c-400a-bdad-01d4658614da"
            }
          ]
        }
      ]
    },
    {
      "name": "Locate",
      "item": [
        {
          "id": "c7cf3b57-2834-4574-a8ff-408d75198105",
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
              "id": "823b44bf-d18e-4c19-8695-a8ca114f691f"
            }
          ]
        },
        {
          "id": "dcd10dc9-8c80-4c0c-838e-6134cd2a6a4d",
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
              "id": "511d779a-0f76-490b-a8c7-e2594aea8e2f"
            }
          ]
        }
      ]
    },
    {
      "name": "Calculate",
      "item": [
        {
          "id": "086a014e-2f88-4bb6-aa02-ac6ac557b7b7",
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
              "id": "b3d9e61b-9642-4bd8-87cb-6d8696a1bbc8"
            }
          ]
        },
        {
          "id": "e84d1536-8d9b-4aef-b23c-8a09af1af3d2",
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
              "id": "d2ab9be2-ee2b-4a99-b07c-fe10faae86c6"
            }
          ]
        }
      ]
    },
    {
      "name": "Detailed",
      "item": [
        {
          "id": "fb0cba38-b341-40fb-afc7-7528fcd88456",
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
              "id": "abb026f6-4d88-4d52-a843-cc8e406f0359"
            }
          ]
        }
      ]
    },
    {
      "name": "Fetch",
      "item": [
        {
          "id": "460f9b9a-727c-4c11-aef4-b822d3885d84",
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
              "id": "6a8e7c73-a0e6-4521-bb52-8e77749117f4"
            }
          ]
        },
        {
          "id": "c8c63382-68f0-437b-bd43-5f81c1726efa",
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
              "id": "9ea69b58-125b-41f6-b315-328fd77a7622"
            }
          ]
        },
        {
          "id": "793a7b44-2378-483a-8b30-61d088fbef76",
          "name": "getSettlement",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.taxamo.com",
              "path": [
                "api/v1/settlement/:quarter"
              ],
              "query": [
                {
                  "key": "currency_code",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "end_month",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "moss_country_code",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "moss_tax_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "refund_date_kind_override",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_month",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tax_country_code",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tax_id",
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
            "description": "Fetch settlement."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50b5a3b7-ba15-4342-aaca-49ede0e8adf3"
            }
          ]
        }
      ]
    },
    {
      "name": "Settlement",
      "item": [
        {
          "id": "b4d823f5-dc3a-4590-9978-e541274a8eab",
          "name": "getSettlementStatsByCountry",
          "request": {
            "url": "http://api.taxamo.com/api/v1/stats/settlement/by_country?date_from=%7B%7D&date_to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Settlement by country."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33d0bc38-3b2f-423e-85e6-643fc098b42c"
            }
          ]
        },
        {
          "id": "c208d8f6-4feb-4933-8ca0-b294f9688c4a",
          "name": "getSettlementStatsByTaxationType",
          "request": {
            "url": "http://api.taxamo.com/api/v1/stats/settlement/by_taxation_type?date_from=%7B%7D&date_to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Settlement by tax type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e518f220-d722-4dda-b4a0-8f1671d32366"
            }
          ]
        },
        {
          "id": "bdec5f02-5f88-414a-a788-7401a9738eb2",
          "name": "getDailySettlementStats",
          "request": {
            "url": "http://api.taxamo.com/api/v1/stats/settlement/daily?date_from=%7B%7D&date_to=%7B%7D&interval=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Settlement stats over time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fb6aaec-05a7-4251-8de1-cd753e52d07c"
            }
          ]
        }
      ]
    },
    {
      "name": "Transaction",
      "item": [
        {
          "id": "70121a31-c82d-49e2-a81a-2b6c68745f4d",
          "name": "getTransactionsStats",
          "request": {
            "url": "http://api.taxamo.com/api/v1/stats/transactions?date_from=%7B%7D&date_to=%7B%7D&interval=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Transaction stats."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35f1a2b9-7775-4090-9cf3-fe9610906113"
            }
          ]
        }
      ]
    }
  ]
}