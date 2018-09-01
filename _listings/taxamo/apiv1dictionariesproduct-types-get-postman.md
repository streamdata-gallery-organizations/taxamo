{
  "info": {
    "name": "Taxamo Product Types",
    "_postman_id": "4627d68a-95ba-4577-9c9d-627b96c091ab",
    "description": "Product types.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Product",
      "item": [
        {
          "id": "f79fca51-f1d3-4e3a-b356-0c8cb5a128c0",
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
              "id": "d9be3fc9-9254-45dd-98eb-13c580b09a98"
            }
          ]
        }
      ]
    }
  ]
}