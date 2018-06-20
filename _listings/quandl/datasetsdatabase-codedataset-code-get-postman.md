{
  "info": {
    "name": "Quandl Get Datasets Database Code Dataset Code",
    "_postman_id": "82afca0d-7749-4e30-8655-50ab9bdc82ee",
    "description": "You can download both data and metadata in a single call, using the following API request. (You can replace .json with .csv or .xml in this request.  If you use .csv, only data will be returned.). In this call, you can customize the dataset object being returned, exactly as in the /data request above.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "31a38a02-c2cc-440b-b74a-1189b28c1be1",
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
              "id": "6fc76a8a-8ed3-47b1-a371-62520daa9d7c"
            }
          ]
        },
        {
          "id": "cd060847-e2d0-4f78-b145-bd8e5be80163",
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
            "description": "To download the data in a dataset, simply append /data to the Quandl code in your API request. (You can replace .csv with .json or .xml in this request). If you request CSV, only the data you requested will be returned.  If you request JSON or XML, both data and input parameters will be returned. You can customize the dataset object being returned by adding various optional parameters to your query. Available parameters are tabulated below: If a datapoint for time t is denoted as y[t] and the transformed data as y’[t], the available transformations are defined as below: y[0] in the above table refers to the starting date for the API call, i.e., the date specified by start_date= or rows=, NOT the starting date of the underlying dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83fed55d-f4dc-402d-9ebf-c3990bb47b4b"
            }
          ]
        },
        {
          "id": "e846c2da-d626-43a9-abe6-864b6eb6befb",
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
              "id": "22b2a00f-421e-4bd8-960f-77b12ec04165"
            }
          ]
        }
      ]
    }
  ]
}