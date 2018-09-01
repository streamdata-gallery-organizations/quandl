{
  "info": {
    "name": "Quandl Get Datasets Database Code Dataset Code Metadata",
    "_postman_id": "a05063d3-bc75-4855-aa57-ecbe3b00a2a9",
    "description": "To download the metadata associated with any dataset object, append /metadata to your API request. (You can replace .csv with .json or .xml in this request). The following metadata fields are available in the response:",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "b4766017-9995-4795-8bbc-ed99114c8241",
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
              "id": "824cfbc5-a6b0-4709-9340-3ce93b8afb0f"
            }
          ]
        }
      ]
    }
  ]
}