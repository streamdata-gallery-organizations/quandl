---
swagger: "2.0"
info:
  title: Quandl
  description: The Quandl API
  version: 1.0.0
host: www.quandl.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /databases:
    get:
      summary: Get Databases
      description: You can search for specific databases on Quandl by making the following
        API request
      operationId: you-can-search-for-specific-databases-on-quandl-by-making-the-following-api-request--the-api-will-re
      parameters:
      - in: query
        name: page
        description: The current page of total available pages you wish to view
      - in: query
        name: per_page
        description: The number of results per page that will be returned
      - in: query
        name: query
        description: You can retrieve all databases related to a search term using
          the query parameter
      responses:
        200:
          description: OK
      tags:
      - market data
definitions: []
x-collection-name: Quandl
x-streamrank:
  polling_total_time_average: ~
  polling_size_download_average: ~
  streaming_total_time_average: ~
  streaming_size_download_average: ~
  change_yes: ~
  change_no: ~
  time_percentage: ~
  size_percentage: ~
  change_percentage: ~
  last_run: ~
  days_run: ~
  minute_run: ~
---