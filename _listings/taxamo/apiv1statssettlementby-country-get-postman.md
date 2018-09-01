{
  "info": {
    "name": "Taxamo Settlement By Country",
    "_postman_id": "2e851235-af56-4452-b795-575e254ba424",
    "description": "Settlement by country.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "3b27feeb-3998-4132-8637-95e607e6708a",
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
              "id": "1d796bd4-f564-412e-bd57-e708c9826e62"
            }
          ]
        }
      ]
    },
    {
      "name": "Settlement",
      "item": [
        {
          "id": "0db5bae8-6672-4a18-9028-5586a76cad71",
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
              "id": "dbf6e0ea-1fa9-45ae-832f-9187603b1ef2"
            }
          ]
        }
      ]
    }
  ]
}