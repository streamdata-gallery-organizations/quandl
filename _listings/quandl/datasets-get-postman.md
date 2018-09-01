{
  "info": {
    "name": "Quandl Get Datasets",
    "_postman_id": "15a6071e-d5e1-4dfc-84cf-52df7665dc66",
    "description": "You can search for individual datasets on Quandl by making the following API request.  The API will return datasets related to your query, as well as datasets that belong to databases related to your query.  Datasets are returned 100 results at a time. You can page through the results using these parameters:",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "81278508-4a29-41bb-8fbf-0edb0cac816d",
          "name": "datasets.database_code.dataset_code.metadata.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.quandl.com",
              "path": [
                "api",
                "v3",
                "datasets/:database_code/:dataset_code/metadata"
              ],
              "query": [
                {
                  "key": "column_names",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "frequency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "newest_available_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "oldest_available_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "premium",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "refreshed_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "database_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "dataset_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To download the metadata associated with any dataset object, append /metadata to your API request. (You can replace .csv with .json or .xml in this request). The following metadata fields are available in the response:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80ab8d8a-37b1-4530-a32e-adff3fa3fbe4"
            }
          ]
        },
        {
          "id": "2cffe0fd-66fd-44aa-8580-8ec66dbd1379",
          "name": "datasets.database_code.dataset_code.data.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.quandl.com",
              "path": [
                "api",
                "v3",
                "datasets/:database_code/:dataset_code/data"
              ],
              "query": [
                {
                  "key": "collapse",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "column_index",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Cumulative",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "end_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Row-on-row",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rows",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Start",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "transform",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "database_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "dataset_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To download the data in a dataset, simply append /data to the Quandl code in your API request. (You can replace .csv with .json or .xml in this request). If you request CSV, only the data you requested will be returned.  If you request JSON or XML, both data and input parameters will be returned. You can customize the dataset object being returned by adding various optional parameters to your query. Available parameters are tabulated below: If a datapoint for time t is denoted as y[t] and the transformed data as y???[t], the available transformations are defined as below: y[0] in the above table refers to the starting date for the API call, i.e., the date specified by start_date= or rows=, NOT the starting date of the underlying dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55d8eba0-fcaa-46d4-92fb-8cff0e78d62d"
            }
          ]
        },
        {
          "id": "1096ddba-733d-4fe8-b7ff-248d7d93c770",
          "name": "datasets.database_code.dataset_code.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.quandl.com",
              "path": [
                "api",
                "v3",
                "datasets/:database_code/:dataset_code"
              ],
              "query": [
                {
                  "key": "collapse",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "column_index",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "end_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "exclude_column_names",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rows",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "transform",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "database_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "dataset_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can download both data and metadata in a single call, using the following API request. (You can replace .json with .csv or .xml in this request.  If you use .csv, only data will be returned.). In this call, you can customize the dataset object being returned, exactly as in the /data request above."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77229142-2bba-458d-bd7f-3afaf585cc64"
            }
          ]
        },
        {
          "id": "7d907215-dfb6-49a6-9962-e9ad9caeed09",
          "name": "datasets.get",
          "request": {
            "url": "http://www.quandl.com/api/v3/datasets?database_code=%7B%7D&page=%7B%7D&per_page=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can search for individual datasets on Quandl by making the following API request.  The API will return datasets related to your query, as well as datasets that belong to databases related to your query.  Datasets are returned 100 results at a time. You can page through the results using these parameters:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18ca1ea4-b308-4bae-90dc-3b0b56533f08"
            }
          ]
        }
      ]
    }
  ]
}