{
  "info": {
    "name": "Taxamo List Payments",
    "_postman_id": "9ce7f781-2417-48aa-9365-0702c4976bce",
    "description": "List payments.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calculate",
      "item": [
        {
          "id": "44f0d402-354e-442c-974c-0b54a71a88fd",
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
              "id": "e6dbe058-18d1-4133-8626-202b9af5e41d"
            }
          ]
        }
      ]
    },
    {
      "name": "Fetch",
      "item": [
        {
          "id": "30714dff-9c58-4eba-bf21-514fbc3f723a",
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
              "id": "5c709016-abad-43f1-9d55-0775ca8db6c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Settlement",
      "item": [
        {
          "id": "62be29a0-d69f-4245-b9dd-617261c7af6f",
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
              "id": "715d9a99-58b9-4c17-8e2a-085baea0910f"
            }
          ]
        },
        {
          "id": "bf38bf0d-8d58-4a8b-8ed1-e2dcf5f98962",
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
              "id": "38d5086b-33b7-45a7-81d7-28b5774a2881"
            }
          ]
        },
        {
          "id": "2f800890-14b8-4b0c-9013-2b1450df3073",
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
              "id": "7537fc82-27af-44d4-8a7f-b76d3fca4b33"
            }
          ]
        },
        {
          "id": "ea927a07-5651-4862-a7d7-e222c280e7ce",
          "name": "getTransactionsStatsByCountry",
          "request": {
            "url": "http://api.taxamo.com/api/v1/stats/transactions/by_country?date_from=%7B%7D&date_to=%7B%7D&global_currency_code=%7B%7D",
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
              "id": "6e0b120d-de9d-48ba-8644-b5ce1134b0a3"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "cc364606-bc2c-4d86-a9cf-314bf6fc1eaa",
          "name": "listPayments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.taxamo.com",
              "path": [
                "api/v1/transactions/:key/payments"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "List payments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5adab472-a7e8-4bb1-aa2a-f93bdd888f67"
            }
          ]
        }
      ]
    }
  ]
}