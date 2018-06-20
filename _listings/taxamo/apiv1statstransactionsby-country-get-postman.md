{
  "info": {
    "name": "Taxamo Settlement By Country",
    "_postman_id": "7d0aa031-303f-463d-8f4b-00695d7081d7",
    "description": "Settlement by country.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "375c078b-5c28-40c2-ba65-9b9034a5c064",
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
              "id": "f9014c2f-114e-4729-b380-d31e079a95d2"
            }
          ]
        }
      ]
    },
    {
      "name": "Settlement",
      "item": [
        {
          "id": "a3f29784-0466-4868-869e-afce4a729bd0",
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
              "id": "d17ec6eb-3d5f-4d71-ad62-592212b0ffd2"
            }
          ]
        },
        {
          "id": "03a82351-a843-4d60-b8b7-e8beb8d9dbf3",
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
              "id": "d931cb12-f085-4e71-a630-0fd3c96584f6"
            }
          ]
        }
      ]
    }
  ]
}