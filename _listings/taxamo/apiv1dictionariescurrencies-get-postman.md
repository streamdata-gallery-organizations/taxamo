{
  "info": {
    "name": "Taxamo Currencies",
    "_postman_id": "e907210f-3885-48fa-b974-11785836f7bb",
    "description": "Currencies.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Currencies",
      "item": [
        {
          "id": "bc01cb32-c78b-4235-985c-2f6ef66ab437",
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
              "id": "d9059bd6-d664-49ee-bf1d-503f7bd9a9ce"
            }
          ]
        }
      ]
    }
  ]
}