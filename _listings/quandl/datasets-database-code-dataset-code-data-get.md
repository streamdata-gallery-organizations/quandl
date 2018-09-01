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
  /datasets/{database_code}/{dataset_code}/data:
    get:
      summary: Get Datasets Data
      description: To download the data in a dataset, simply append /data to the Quandl
        code in your API request
      operationId: to-download-the-data-in-a-dataset-simply-append-data-to-the-quandl-code-in-your-api-request-you-can-
      parameters:
      - in: query
        name: collapse
        description: Parameters to indicate the desired frequency
      - in: query
        name: column_index
        description: Request a specific column by passing the column_index=n parameter
      - in: query
        name: Cumulative
        description: "y\u2019[t] = y[t] +y[t-1] + \u2026 + y[0]"
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
        name: limit
        description: You can use limit=n to get only the first n rows of your dataset
      - in: query
        name: order
        description: Select the sort order by passing the parameter order=asc|desc
      - in: query
        name: Row-on-row
        description: "y\u2019[t] = y[t] - y[t-1]"
      - in: query
        name: rows
        description: You can use rows=n to get only the first n rows of your dataset
      - in: query
        name: Start
        description: "y\u2019[t] = (y[t]/y[0]) * 100"
      - in: query
        name: start_date
        description: Retrieve data within a specific date range, by setting start
          dates for your query
      - in: query
        name: transform
        description: Perform  calculations on your data prior to downloading
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