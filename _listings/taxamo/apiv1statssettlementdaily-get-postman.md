{
  "info": {
    "name": "Taxamo Settlement Stats Over Time",
    "_postman_id": "5ebf4b33-ddfd-4628-8f54-b786de2380f9",
    "description": "Settlement stats over time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calculate",
      "item": [
        {
          "id": "6d695d89-9967-4c19-9d77-88909c855166",
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
              "id": "cba3f6fc-5267-4e06-958e-2a092eaf1818"
            }
          ]
        }
      ]
    },
    {
      "name": "Fetch",
      "item": [
        {
          "id": "58470732-a17b-47e0-9664-7b4eb38b5bb9",
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
              "id": "be418906-b7e1-457d-8080-af7d362a9d6e"
            }
          ]
        }
      ]
    },
    {
      "name": "Settlement",
      "item": [
        {
          "id": "e6b8afe4-1b1a-47dd-9161-d510ad33d306",
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
              "id": "a93f6545-b4f1-4948-a962-b7775668c961"
            }
          ]
        },
        {
          "id": "bc845ef3-efd3-4f30-b102-2e2b80e96135",
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
              "id": "b52e57a4-1e2a-4d50-b006-3d947120129e"
            }
          ]
        },
        {
          "id": "51c169f7-4e90-4000-9f6e-2e9aaf2aa20f",
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
              "id": "d116659b-158b-4e45-977f-947865d95840"
            }
          ]
        }
      ]
    }
  ]
}