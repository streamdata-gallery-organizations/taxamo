---
swagger: "2.0"
x-collection-name: Taxamo
x-complete: 0
info:
  title: Taxamo Settlement By Tax Type
  description: Settlement by tax type.
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
  /api/v1/geoip:
    get:
      summary: Locate IP Address
      description: Locate ip address.
      operationId: locateMyIP
      x-api-path-slug: apiv1geoip-get
      responses:
        200:
          description: OK
      tags:
      - Locate
      - IP
      - Ress
  /api/v1/geoip/{ip}:
    get:
      summary: Locate Provided IP Address
      description: Locate provided ip address.
      operationId: locateGivenIP
      x-api-path-slug: apiv1geoipip-get
      parameters:
      - in: path
        name: ip
        description: IP address
      responses:
        200:
          description: OK
      tags:
      - Locate
      - Provided
      - IP
      - Ress
  /api/v1/reports/domestic/summary:
    get:
      summary: Calculate Domestic Summary
      description: Calculate domestic summary.
      operationId: getDomesticSummaryReport
      x-api-path-slug: apiv1reportsdomesticsummary-get
      parameters:
      - in: query
        name: country_code
        description: ISO 2-letter country code which will be used for determining
          which country is domestic
      - in: query
        name: currency_code
        description: ISO 3-letter currency code, e
      - in: query
        name: end_month
        description: Period end month in yyyy-MM format
      - in: query
        name: format
        description: Output format
      - in: query
        name: fx_date_type
        description: Which date should be used for FX
      - in: query
        name: start_month
        description: Period start month in yyyy-MM format
      responses:
        200:
          description: OK
      tags:
      - Calculate
      - Domestic
      - Summary
  /api/v1/reports/eu/vies:
    get:
      summary: Calculate EU VIES Report
      description: Calculate eu vies report.
      operationId: getEuViesReport
      x-api-path-slug: apiv1reportseuvies-get
      parameters:
      - in: query
        name: currency_code
        description: ISO 3-letter currency code, e
      - in: query
        name: end_month
        description: Period end month in yyyy-MM format
      - in: query
        name: eu_country_code
        description: ISO 2-letter country code which will be used for determining
          which country is domestic
      - in: query
        name: format
        description: Output format
      - in: query
        name: fx_date_type
        description: Which date should be used for FX
      - in: query
        name: lff_sequence_number
        description: Sequence number used to generate report in Large Filer Format
      - in: query
        name: period_length
        description: Length of report period
      - in: query
        name: start_month
        description: Period start month in yyyy-MM format
      - in: query
        name: tax_id
        description: MOSS-assigned tax ID - if not provided, merchants national tax
          number will be used
      - in: query
        name: transformation
        description: Which transformation should be applied
      responses:
        200:
          description: OK
      tags:
      - Calculate
      - EU
      - VIES
      - Report
  /api/v1/settlement/detailed_refunds:
    get:
      summary: Detailed Refunds
      description: Detailed refunds.
      operationId: getDetailedRefunds
      x-api-path-slug: apiv1settlementdetailed-refunds-get
      parameters:
      - in: query
        name: country_codes
        description: Comma separated list of 2-letter country codes
      - in: query
        name: date_from
        description: Take only refunds issued at or after the date
      - in: query
        name: date_to
        description: Take only refunds issued at or before the date
      - in: query
        name: format
        description: Output format
      - in: query
        name: limit
        description: Limit (no more than 1000, defaults to 100)
      - in: query
        name: offset
        description: Offset
      responses:
        200:
          description: OK
      tags:
      - Detailed
      - Refunds
  /api/v1/settlement/refunds:
    get:
      summary: Fetch Refunds
      description: Fetch refunds.
      operationId: getRefunds
      x-api-path-slug: apiv1settlementrefunds-get
      parameters:
      - in: query
        name: date_from
        description: Take only refunds issued at or after the date
      - in: query
        name: format
        description: Output format
      - in: query
        name: moss_country_code
        description: MOSS country code, used to determine currency
      - in: query
        name: tax_region
        description: Tax region key, defaults to EU for backwards compatibility
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Refunds
  /api/v1/settlement/summary/{quarter}:
    get:
      summary: Fetch Summary
      description: Fetch summary.
      operationId: getSettlementSummary
      x-api-path-slug: apiv1settlementsummaryquarter-get
      parameters:
      - in: query
        name: end_month
        description: Period end month in yyyy-MM format
      - in: query
        name: moss_country_code
        description: MOSS country code, used to determine currency
      - in: path
        name: quarter
        description: Quarter in yyyy-MM format
      - in: query
        name: start_month
        description: Period start month in yyyy-MM format
      - in: query
        name: tax_region
        description: Tax region key
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Summary
  /api/v1/settlement/{quarter}:
    get:
      summary: Fetch Settlement
      description: Fetch settlement.
      operationId: getSettlement
      x-api-path-slug: apiv1settlementquarter-get
      parameters:
      - in: query
        name: currency_code
        description: ISO 3-letter currency code, e
      - in: query
        name: end_month
        description: Period end month in yyyy-MM format
      - in: query
        name: format
        description: Output format
      - in: query
        name: moss_country_code
        description: MOSS country code, used to determine currency/region
      - in: query
        name: moss_tax_id
        description: MOSS-assigned tax ID - if not provided, merchants national tax
          number will be used
      - in: path
        name: quarter
        description: Quarter in yyyy-MM format
      - in: query
        name: refund_date_kind_override
        description: Set to order_date to show only refunds for the transactions in
          the selected reporting period
      - in: query
        name: start_month
        description: Period start month in yyyy-MM format
      - in: query
        name: tax_country_code
        description: Tax entity country code, used to determine currency/region
      - in: query
        name: tax_id
        description: MOSS-assigned tax ID - if not provided, merchants national tax
          number will be used
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Settlement
  /api/v1/stats/settlement/by_country:
    get:
      summary: Settlement By Country
      description: Settlement by country.
      operationId: getSettlementStatsByCountry
      x-api-path-slug: apiv1statssettlementby-country-get
      parameters:
      - in: query
        name: date_from
        description: Date from in yyyy-MM format
      - in: query
        name: date_to
        description: Date to in yyyy-MM format
      responses:
        200:
          description: OK
      tags:
      - Settlement
      - Country
  /api/v1/stats/settlement/by_taxation_type:
    get:
      summary: Settlement By Tax Type
      description: Settlement by tax type.
      operationId: getSettlementStatsByTaxationType
      x-api-path-slug: apiv1statssettlementby-taxation-type-get
      parameters:
      - in: query
        name: date_from
        description: Date from in yyyy-MM format
      - in: query
        name: date_to
        description: Date to in yyyy-MM format
      responses:
        200:
          description: OK
      tags:
      - Settlement
      - Tax
      - Type
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