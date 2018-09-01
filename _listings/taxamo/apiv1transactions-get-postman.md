{
  "info": {
    "name": "Taxamo Browse Transactions",
    "_postman_id": "2eb2f1cb-5c93-4074-aa60-596e86443916",
    "description": "Browse transactions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Browse",
      "item": [
        {
          "id": "ab1a6611-9cf2-4e44-a299-558233fd0dc5",
          "name": "listTransactions",
          "request": {
            "url": "http://api.taxamo.com/api/v1/transactions?currency_code=%7B%7D&filter_text=%7B%7D&format=%7B%7D&has_note=%7B%7D&invoice_number=%7B%7D&key_or_custom_id=%7B%7D&limit=%7B%7D&offset=%7B%7D&order_date_from=%7B%7D&order_date_to=%7B%7D&original_transaction_key=%7B%7D&sort_reverse=%7B%7D&statuses=%7B%7D&tax_country_code=%7B%7D&tax_country_codes=%7B%7D&total_amount_greater_than=%7B%7D&total_amount_less_than=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Browse transactions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53fc5e76-945d-4061-8f1d-234585684ea2"
            }
          ]
        }
      ]
    }
  ]
}