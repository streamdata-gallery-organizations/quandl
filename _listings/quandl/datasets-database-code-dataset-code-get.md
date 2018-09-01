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
  /datasets/{database_code}/{dataset_code}:
    get:
      summary: Get Dataset
      description: You can download both data and metadata in a single call, using
        the following API request
      operationId: you-can-download-both-data-and-metadata-in-a-single-call-using-the-following-api-request-you-can-rep
      parameters:
      - in: query
        name: collapse
        description: Parameters to indicate the desired frequency
      - in: query
        name: column_index
        description: Request a specific column by passing the column_index=n parameter
      - in: path
        name: database_code
        description: Each database on Quandl has a unique database code
      - in: path
        name: dataset_code
        description: Each dataset on Quandl has a unique dataset code
      - in: query
        name: end_date
        description: Retrieve data within a specific date range, by setting end dates
          for your query
      - in: query
        name: exclude_column_names
        description: Request data without column names by passing the exclude_column_names=true
          parameter
      - in: query
        name: limit
        description: You can use limit=n to get only the first n rows of your dataset
      - in: query
        name: order
        description: You can select the sort order by passing the parameter order=asc|desc
      - in: query
        name: rows
        description: You can use rows=n to get only the first n rows of your dataset
      - in: query
        name: start_date
        description: Retrieve data within a specific date range, by setting start
          for your query
      - in: query
        name: transform
        description: Perform  calculations on your data prior to downloading
      responses:
        200:
          description: OK
      tags:
      - market data
      - csv
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