---
swagger: "2.0"
x-collection-name: Quandl
x-complete: 0
info:
  title: Quandl API Download Codes
  description: You can download a list of all dataset codes in a database in a single
    call, by appending /codes to your database request. The call will return a ZIP
    file containing a CSV.
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
      description: 'You can search for specific databases on Quandl by making the
        following API request.  The API will return databases related to your query.
        Databases are returned 100 results at a time. You can page through the results
        using these parameters:'
      operationId: you-can-search-for-specific-databases-on-quandl-by-making-the-following-api-request--the-api-will-re
      x-api-path-slug: databases-get
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
      - Market Data
  /databases/{database_code}:
    get:
      summary: Get Database
      description: This call returns descriptive metadata for the specified database.
      operationId: this-call-returns-descriptive-metadata-for-the-specified-database
      x-api-path-slug: databasesdatabase-code-get
      parameters:
      - in: path
        name: database_code
        description: The unique database code on Quandl (ex
      responses:
        200:
          description: OK
      tags:
      - Market Data
  /databases/{database_code}/codes:
    get:
      summary: Download Codes
      description: You can download a list of all dataset codes in a database in a
        single call, by appending /codes to your database request. The call will return
        a ZIP file containing a CSV.
      operationId: you-can-download-a-list-of-all-dataset-codes-in-a-database-in-a-single-call-by-appending-codes-to-yo
      x-api-path-slug: databasesdatabase-codecodes-get
      parameters:
      - in: path
        name: database_code
        description: The unique database code on Quandl (ex
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - CSV
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