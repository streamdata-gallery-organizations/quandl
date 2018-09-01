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
  /datasets:
    get:
      summary: Get Datasets
      description: You can search for individual datasets on Quandl by making the
        following API request
      operationId: you-can-search-for-individual-datasets-on-quandl-by-making-the-following-api-request--the-api-will-r
      parameters:
      - in: query
        name: database_code
        description: You can restrict your search to a specific database by including
          a Quandl database code
      - in: query
        name: page
        description: The current page of total available pages you wish to view
      - in: query
        name: per_page
        description: The number of results per page that will be returned
      - in: query
        name: query
        description: You can retrieve all datasets related to a search term using
          the query parameter
      responses:
        200:
          description: OK
      tags:
      - market data
definitions: []
x-collection-name: Quandl
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