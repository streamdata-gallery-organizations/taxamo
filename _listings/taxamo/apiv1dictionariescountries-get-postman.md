{
  "info": {
    "name": "Taxamo Countries",
    "_postman_id": "04cef44c-d50a-4c00-9b99-a0e778f6b68a",
    "description": "Countries.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "fead6968-2fd5-413b-b1dc-a82e0bd4d339",
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
              "id": "3c551180-71df-4793-8e5b-90ab1d20033e"
            }
          ]
        }
      ]
    }
  ]
}