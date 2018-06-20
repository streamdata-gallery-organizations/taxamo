{
  "info": {
    "name": "Taxamo Calculate Domestic Summary",
    "_postman_id": "52ed74e6-bd07-4734-ad9f-524e3c208d90",
    "description": "Calculate domestic summary.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calculate",
      "item": [
        {
          "id": "a257599b-70de-46fb-a002-5b3bfcf38bad",
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
              "id": "511f465b-afee-481e-9b5c-0afac7801fe2"
            }
          ]
        }
      ]
    }
  ]
}