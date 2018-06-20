{
  "info": {
    "name": "Taxamo Detailed Refunds",
    "_postman_id": "2e34e103-7f38-49ff-8da6-6d4388fa313d",
    "description": "Detailed refunds.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Detailed",
      "item": [
        {
          "id": "6aae41de-bc8a-4e3d-a75e-37dfeb51ab1c",
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
              "id": "b8bcac51-0478-4f90-a9ec-29120683b740"
            }
          ]
        }
      ]
    }
  ]
}