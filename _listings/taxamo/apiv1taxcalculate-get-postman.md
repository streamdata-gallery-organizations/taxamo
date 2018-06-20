{
  "info": {
    "name": "Taxamo Simple Tax",
    "_postman_id": "4524ffaa-1334-43ee-9b25-af4a5fccf76b",
    "description": "Simple tax.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "0a6d54ef-cece-4d63-98d4-79b7b7f5f72a",
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
              "id": "6f8615f5-560c-44f5-a68e-a3302977689e"
            }
          ]
        }
      ]
    },
    {
      "name": "Currencies",
      "item": [
        {
          "id": "9ddce436-2050-4cac-9f6e-660768dca54b",
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
              "id": "91bc1a48-a1a9-4df2-8e2a-f469bc985631"
            }
          ]
        }
      ]
    },
    {
      "name": "Product",
      "item": [
        {
          "id": "7c4871ae-de9c-47f0-be92-99851eb36a0b",
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
              "id": "a3b7d5bf-fa86-48a1-9544-9b2a93931c3e"
            }
          ]
        }
      ]
    },
    {
      "name": "Locate",
      "item": [
        {
          "id": "3b1a4c96-4097-40a6-a6ee-dc37268a3142",
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
              "id": "ad225ae0-057d-4780-ba6a-80201f8dc18b"
            }
          ]
        },
        {
          "id": "3b5ced87-f2d2-4049-a8b0-f1e43304b483",
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
              "id": "c9aa089a-801d-4659-8b19-9947df0b0825"
            }
          ]
        }
      ]
    },
    {
      "name": "Calculate",
      "item": [
        {
          "id": "be4936cb-9835-49b0-adfd-27c59d26aeed",
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
              "id": "811c4419-d643-4338-b31e-598a05eccc17"
            }
          ]
        },
        {
          "id": "e792925f-ee78-4651-8751-32d40e7275b1",
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
              "id": "480d6812-8526-4e9a-8424-277a6ed6619a"
            }
          ]
        }
      ]
    },
    {
      "name": "Detailed",
      "item": [
        {
          "id": "a9189f00-a1f8-41cb-8031-b675678c7b90",
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
              "id": "1f9f28f4-240e-4081-8445-832fb6711b86"
            }
          ]
        }
      ]
    },
    {
      "name": "Fetch",
      "item": [
        {
          "id": "fde8e4b3-50b8-40bb-9b85-a38d160a50ac",
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
              "id": "38d39d6f-3db2-4ca2-8b12-8b7c05cc6b1a"
            }
          ]
        },
        {
          "id": "b3f7bd51-98b1-43da-9d9f-c957965bda0a",
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
              "id": "5fba1aab-d15a-49a9-822a-b3e22ffb4ff2"
            }
          ]
        },
        {
          "id": "ff2a3457-8bd5-48a8-925c-ad6e28f996ce",
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
              "id": "f59870ca-5a63-41ef-8e91-525d1c2b700a"
            }
          ]
        }
      ]
    },
    {
      "name": "Settlement",
      "item": [
        {
          "id": "2cb59d4f-1784-4439-ba7a-106afd8d4141",
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
              "id": "012d95be-a244-4a20-9622-4b095c06de84"
            }
          ]
        },
        {
          "id": "6d99f0a9-71d4-4de9-b4c9-f4e55db809f5",
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
              "id": "35bb2f33-6f6b-4ad5-84b1-667477bb73a0"
            }
          ]
        },
        {
          "id": "d0d9070a-5a8e-4218-988a-6d5e6b19c2c1",
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
              "id": "85d10834-6c39-4fca-bedb-7ed5cdda121a"
            }
          ]
        },
        {
          "id": "295b7dc2-dcf7-443a-bf89-0ff302e78c4e",
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
              "id": "6c728736-0730-496a-b1c3-b4ca2e6fa43f"
            }
          ]
        }
      ]
    },
    {
      "name": "Transaction",
      "item": [
        {
          "id": "77555693-27bd-473c-b945-aac31dea02ff",
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
              "id": "8fbc733d-f78a-434e-8f91-d03af7012dee"
            }
          ]
        }
      ]
    },
    {
      "name": "Simple",
      "item": [
        {
          "id": "ca7254a8-da83-4dda-b553-9fe4821d36ce",
          "name": "calculateSimpleTax",
          "request": {
            "url": "http://api.taxamo.com/api/v1/tax/calculate?amount=%7B%7D&billing_country_code=%7B%7D&buyer_credit_card_prefix=%7B%7D&buyer_tax_number=%7B%7D&currency_code=%7B%7D&force_country_code=%7B%7D&invoice_address_city=%7B%7D&invoice_address_postal_code=%7B%7D&invoice_address_region=%7B%7D&order_date=%7B%7D&product_type=%7B%7D&quantity=%7B%7D&tax_deducted=%7B%7D&total_amount=%7B%7D&unit_price=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Simple tax."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab29719c-903f-4d87-8ae2-765da89cc51b"
            }
          ]
        }
      ]
    }
  ]
}