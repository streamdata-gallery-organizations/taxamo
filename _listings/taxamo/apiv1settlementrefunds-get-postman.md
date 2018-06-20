{
  "info": {
    "name": "Taxamo Fetch Refunds",
    "_postman_id": "8f18c697-74b2-49d5-9bac-1899d3b002aa",
    "description": "Fetch refunds.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Detailed",
      "item": [
        {
          "id": "b92815dc-067e-4097-a66d-80fc99221b72",
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
              "id": "b9efc198-54d9-4b2d-91c6-20a33ce8ff7a"
            }
          ]
        }
      ]
    },
    {
      "name": "Fetch",
      "item": [
        {
          "id": "5f5b9d60-dd56-4fa0-8a00-70a10eb250a4",
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
              "id": "e4578dc7-a855-4261-84a7-4daff6d5e664"
            }
          ]
        }
      ]
    }
  ]
}