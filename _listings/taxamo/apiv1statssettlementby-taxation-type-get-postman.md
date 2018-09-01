{
  "info": {
    "name": "Taxamo Settlement By Tax Type",
    "_postman_id": "34d18811-d01a-4b97-a34b-946fed2f684c",
    "description": "Settlement by tax type.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calculate",
      "item": [
        {
          "id": "7e97e1a2-ab42-40bf-bd3f-0d39c7418785",
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
              "id": "e6cac66b-99d7-4673-9dcf-27ceffa6a58c"
            }
          ]
        }
      ]
    },
    {
      "name": "Fetch",
      "item": [
        {
          "id": "ee3cda18-f44f-4439-979c-12be3d4ef773",
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
              "id": "c2dddabf-fa60-44c0-9197-e9a69d27184d"
            }
          ]
        }
      ]
    },
    {
      "name": "Settlement",
      "item": [
        {
          "id": "896dcddd-320e-4571-91eb-954d39f466e5",
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
              "id": "31ab01ef-2a78-4072-a77a-30d054d9c544"
            }
          ]
        },
        {
          "id": "a3cf54e4-8c70-4a40-8132-d9ce8fad9056",
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
              "id": "29ca89db-ea45-4262-9401-0bc469a602e6"
            }
          ]
        }
      ]
    }
  ]
}