---
swagger: "2.0"
x-collection-name: Quandl
x-complete: 0
info:
  title: Quandl Get Datasets Database Code Dataset Code Data
  description: "To download the data in a dataset, simply append /data to the Quandl
    code in your API request. (You can replace .csv with .json or .xml in this request).
    If you request CSV, only the data you requested will be returned.  If you request
    JSON or XML, both data and input parameters will be returned. You can customize
    the dataset object being returned by adding various optional parameters to your
    query. Available parameters are tabulated below: If a datapoint for time t is
    denoted as y[t] and the transformed data as y\u2019[t], the available transformations
    are defined as below: y[0] in the above table refers to the starting date for
    the API call, i.e., the date specified by start_date= or rows=, NOT the starting
    date of the underlying dataset."
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
  /datasets/{database_code}/{dataset_code}/metadata:
    get:
      summary: Get Datasets Database Code Dataset Code Metadata
      description: 'To download the metadata associated with any dataset object, append
        /metadata to your API request. (You can replace .csv with .json or .xml in
        this request). The following metadata fields are available in the response:'
      operationId: datasets.database_code.dataset_code.metadata.get
      x-api-path-slug: datasetsdatabase-codedataset-codemetadata-get
      parameters:
      - in: query
        name: column_names
      - in: path
        name: database_code
        description: The unique database code on Quandl (ex
      - in: path
        name: dataset_code
        description: The unique dataset code on Quandl (ex
      - in: query
        name: description
      - in: query
        name: frequency
      - in: query
        name: name
      - in: query
        name: newest_available_date
      - in: query
        name: oldest_available_date
      - in: query
        name: premium
      - in: query
        name: refreshed_at
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Datasets
      - Database
      - Code
      - Dataset
      - Code
      - Metadata
  /datasets/{database_code}/{dataset_code}/data:
    get:
      summary: Get Datasets Database Code Dataset Code Data
      description: "To download the data in a dataset, simply append /data to the
        Quandl code in your API request. (You can replace .csv with .json or .xml
        in this request). If you request CSV, only the data you requested will be
        returned.  If you request JSON or XML, both data and input parameters will
        be returned. You can customize the dataset object being returned by adding
        various optional parameters to your query. Available parameters are tabulated
        below: If a datapoint for time t is denoted as y[t] and the transformed data
        as y\u2019[t], the available transformations are defined as below: y[0] in
        the above table refers to the starting date for the API call, i.e., the date
        specified by start_date= or rows=, NOT the starting date of the underlying
        dataset."
      operationId: datasets.database_code.dataset_code.data.get
      x-api-path-slug: datasetsdatabase-codedataset-codedata-get
      parameters:
      - in: query
        name: collapse
        description: Parameters to indicate the desired frequency
      - in: query
        name: column_index
        description: Request a specific column by passing the column_index=n parameter
      - in: query
        name: Cumulative
        description: y[t] = y[t] +y[t-1] +  + y[0]
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
        description: y[t] = y[t] - y[t-1]
      - in: query
        name: rows
        description: You can use rows=n to get only the first n rows of your dataset
      - in: query
        name: Start
        description: y[t] = (y[t]/y[0]) * 100
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
      - Market Data
      - Datasets
      - Database
      - Code
      - Dataset
      - Code
      - Data
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