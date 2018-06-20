{
  "info": {
    "name": "Quandl Get Databases Database Code Data",
    "_postman_id": "5d4fa591-1033-43f7-9241-dfa508347d9e",
    "description": "You can download all the data in a premium database in a single call, by appending /data to your database request. You can specify whether you want the entire history, or merely the last day’s worth of updates, by setting the correct query parameters.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "d5812bed-b8ff-453d-b2c6-6314426347ce",
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
              "id": "d55491c5-327e-4061-a630-8cc73cb8a0dd"
            }
          ]
        },
        {
          "id": "637e0e53-a8ac-467a-bbc0-e0d74e6c51ea",
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
              "id": "673c8efa-f345-4ea8-a8f8-672c3e5db41c"
            }
          ]
        },
        {
          "id": "4987ad91-2105-4447-98bc-445a09cd3c29",
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
              "id": "03394c4b-d4d8-43b7-b866-54a2721dd27a"
            }
          ]
        },
        {
          "id": "be42a209-1f97-4ade-88c9-f489c6809358",
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
              "id": "5fa6ca9e-8242-4b2a-a077-270a22b92f3e"
            }
          ]
        },
        {
          "id": "3a18a9c6-8796-4251-956a-f93be2767a66",
          "name": "databases.database_code.data.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.quandl.com",
              "path": [
                "api",
                "v3",
                "databases/:database_code/data"
              ],
              "query": [
                {
                  "key": "download_type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "database_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can download all the data in a premium database in a single call, by appending /data to your database request. You can specify whether you want the entire history, or merely the last day’s worth of updates, by setting the correct query parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc30b049-d995-432a-99d0-3d1c90def15b"
            }
          ]
        }
      ]
    }
  ]
}