{
  "info": {
    "name": "Taxamo Fetch Settlement",
    "_postman_id": "720566de-975a-41fa-b252-7b0657c4f69a",
    "description": "Fetch settlement.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calculate",
      "item": [
        {
          "id": "007a6407-1848-4b43-8750-fda0984db9e6",
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
              "id": "8130fdb6-e43e-423e-b1fe-c094bc737015"
            }
          ]
        }
      ]
    },
    {
      "name": "Fetch",
      "item": [
        {
          "id": "5ab08aa8-29d7-4f09-bc03-bb47d52562b9",
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
              "id": "489e6e97-1f95-48de-a199-bd26df9fe50d"
            }
          ]
        }
      ]
    }
  ]
}