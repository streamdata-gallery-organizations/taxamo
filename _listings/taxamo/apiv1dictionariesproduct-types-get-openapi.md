---
swagger: "2.0"
x-collection-name: taxamo
x-complete: 0
info:
  title: Taxamo Product Types
  description: Product types.
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/dictionaries/countries:
    get:
      summary: Countries
      description: Countries.
      operationId: getCountriesDict
      x-api-path-slug: apiv1dictionariescountries-get
      parameters:
      - in: query
        name: tax_supported
        description: Should only countries with tax supported be listed?
      responses:
        200:
          description: OK
      tags:
      - Countries
  /api/v1/dictionaries/currencies:
    get:
      summary: Currencies
      description: Currencies.
      operationId: getCurrenciesDict
      x-api-path-slug: apiv1dictionariescurrencies-get
      responses:
        200:
          description: OK
      tags:
      - Currencies
  /api/v1/dictionaries/product_types:
    get:
      summary: Product Types
      description: Product types.
      operationId: getProductTypesDict
      x-api-path-slug: apiv1dictionariesproduct-types-get
      responses:
        200:
          description: OK
      tags:
      - Product
      - Types
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---