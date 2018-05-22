---
swagger: "2.0"
x-collection-name: Quandl
x-complete: 0
info:
  title: Quandl API Get Datasets Metadata
  description: 'To download the metadata associated with any dataset object, append
    /metadata to your API request. (You can replace .csv with .json or .xml in this
    request). The following metadata fields are available in the response:'
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
  /databases/{database_code}/data:
    get:
      summary: Get Data
      description: "You can download all the data in a premium database in a single
        call, by appending /data to your database request. You can specify whether
        you want the entire history, or merely the last day\u2019s worth of updates,
        by setting the correct query parameters."
      operationId: you-can-download-all-the-data-in-a-premium-database-in-a-single-call-by-appending-data-to-your-datab
      x-api-path-slug: databasesdatabase-codedata-get
      parameters:
      - in: path
        name: database_code
        description: The unique database code on Quandl (ex
      - in: query
        name: download_type
        description: Data returned can be either partial or complete
      responses:
        200:
          description: OK
      tags:
      - Market Data
  /datasets:
    get:
      summary: Get Datasets
      description: 'You can search for individual datasets on Quandl by making the
        following API request.  The API will return datasets related to your query,
        as well as datasets that belong to databases related to your query.  Datasets
        are returned 100 results at a time. You can page through the results using
        these parameters:'
      operationId: you-can-search-for-individual-datasets-on-quandl-by-making-the-following-api-request--the-api-will-r
      x-api-path-slug: datasets-get
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
      - Market Data
  /datasets/{database_code}/{dataset_code}:
    get:
      summary: Get Dataset
      description: You can download both data and metadata in a single call, using
        the following API request. (You can replace .json with .csv or .xml in this
        request.  If you use .csv, only data will be returned.). In this call, you
        can customize the dataset object being returned, exactly as in the /data request
        above.
      operationId: you-can-download-both-data-and-metadata-in-a-single-call-using-the-following-api-request-you-can-rep
      x-api-path-slug: datasetsdatabase-codedataset-code-get
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
      - Market Data
      - CSV
  /datasets/{database_code}/{dataset_code}/data:
    get:
      summary: Get Datasets Data
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
      operationId: to-download-the-data-in-a-dataset-simply-append-data-to-the-quandl-code-in-your-api-request-you-can-
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
      - Market Data
  /datasets/{database_code}/{dataset_code}/metadata:
    get:
      summary: Get Datasets Metadata
      description: 'To download the metadata associated with any dataset object, append
        /metadata to your API request. (You can replace .csv with .json or .xml in
        this request). The following metadata fields are available in the response:'
      operationId: to-download-the-metadata-associated-with-any-dataset-object-append-metadata-to-your-api-request-you-
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