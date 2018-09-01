---
name: Quandl
x-slug: quandl
description: Quandl delivers financial data to users in the format they want. Access
  thousands of databases via the Quandl API or in your tool of choice.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11440-quandl.jpg
x-kinRank: "8"
x-alexaRank: "53781"
tags: Quandl
created: "2018-08-31"
modified: "2018-08-31"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/apis.md
specificationVersion: "0.14"
apis:
- name: Quandl - Get Datasets Database Code Dataset Code Metadata
  x-api-slug: datasetsdatabase-codedataset-codemetadata-get
  description: 'To download the metadata associated with any dataset object, append
    /metadata to your API request. (You can replace .csv with .json or .xml in this
    request). The following metadata fields are available in the response:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11440-quandl.jpg
  humanURL: http://quandl.com
  baseURL: https://www.quandl.com//api/v3
  tags: Finance, Data, Finance, Target, Imports, Stack Network, internet, Technology,
    SaaS, Enterprise, Market Data, Sign In With Github, Sign In With Google, Sign
    In With LinkedIn, Have API Key, Visualizations, General Data, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/datasetsdatabase-codedataset-codemetadata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/datasetsdatabase-codedataset-codemetadata-get-openapi.md
- name: Quandl - Get Datasets Database Code Dataset Code Data
  x-api-slug: datasetsdatabase-codedataset-codedata-get
  description: 'To download the data in a dataset, simply append /data to the Quandl
    code in your API request. (You can replace .csv with .json or .xml in this request).
    If you request CSV, only the data you requested will be returned.  If you request
    JSON or XML, both data and input parameters will be returned. You can customize
    the dataset object being returned by adding various optional parameters to your
    query. Available parameters are tabulated below: If a datapoint for time t is
    denoted as y[t] and the transformed data as y???[t], the available transformations
    are defined as below: y[0] in the above table refers to the starting date for
    the API call, i.e., the date specified by start_date= or rows=, NOT the starting
    date of the underlying dataset.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11440-quandl.jpg
  humanURL: http://quandl.com
  baseURL: https://www.quandl.com//api/v3
  tags: Finance, Data, Finance, Target, Imports, Stack Network, internet, Technology,
    SaaS, Enterprise, Market Data, Sign In With Github, Sign In With Google, Sign
    In With LinkedIn, Have API Key, Visualizations, General Data, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/datasetsdatabase-codedataset-codedata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/datasetsdatabase-codedataset-codedata-get-openapi.md
- name: Quandl - Get Datasets Database Code Dataset Code
  x-api-slug: datasetsdatabase-codedataset-code-get
  description: You can download both data and metadata in a single call, using the
    following API request. (You can replace .json with .csv or .xml in this request.  If
    you use .csv, only data will be returned.). In this call, you can customize the
    dataset object being returned, exactly as in the /data request above.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11440-quandl.jpg
  humanURL: http://quandl.com
  baseURL: https://www.quandl.com//api/v3
  tags: Finance, Data, Finance, Target, Imports, Stack Network, internet, Technology,
    SaaS, Enterprise, Market Data, Sign In With Github, Sign In With Google, Sign
    In With LinkedIn, Have API Key, Visualizations, General Data, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/datasetsdatabase-codedataset-code-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/datasetsdatabase-codedataset-code-get-openapi.md
- name: Quandl - Get Datasets
  x-api-slug: datasets-get
  description: 'You can search for individual datasets on Quandl by making the following
    API request.  The API will return datasets related to your query, as well as datasets
    that belong to databases related to your query.  Datasets are returned 100 results
    at a time. You can page through the results using these parameters:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11440-quandl.jpg
  humanURL: http://quandl.com
  baseURL: https://www.quandl.com//api/v3
  tags: Finance, Data, Finance, Target, Imports, Stack Network, internet, Technology,
    SaaS, Enterprise, Market Data, Sign In With Github, Sign In With Google, Sign
    In With LinkedIn, Have API Key, Visualizations, General Data, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/datasets-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/datasets-get-openapi.md
- name: Quandl - Get Databases Database Code Data
  x-api-slug: databasesdatabase-codedata-get
  description: You can download all the data in a premium database in a single call,
    by appending /data to your database request. You can specify whether you want
    the entire history, or merely the last day???s worth of updates, by setting the
    correct query parameters.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11440-quandl.jpg
  humanURL: http://quandl.com
  baseURL: https://www.quandl.com//api/v3
  tags: Finance, Data, Finance, Target, Imports, Stack Network, internet, Technology,
    SaaS, Enterprise, Market Data, Sign In With Github, Sign In With Google, Sign
    In With LinkedIn, Have API Key, Visualizations, General Data, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/databasesdatabase-codedata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/databasesdatabase-codedata-get-openapi.md
- name: Quandl - Get Databases Database Code Codes
  x-api-slug: databasesdatabase-codecodes-get
  description: You can download a list of all dataset codes in a database in a single
    call, by appending /codes to your database request. The call will return a ZIP
    file containing a CSV.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11440-quandl.jpg
  humanURL: http://quandl.com
  baseURL: https://www.quandl.com//api/v3
  tags: Finance, Data, Finance, Target, Imports, Stack Network, internet, Technology,
    SaaS, Enterprise, Market Data, Sign In With Github, Sign In With Google, Sign
    In With LinkedIn, Have API Key, Visualizations, General Data, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/databasesdatabase-codecodes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/databasesdatabase-codecodes-get-openapi.md
- name: Quandl - Get Databases Database Code
  x-api-slug: databasesdatabase-code-get
  description: This call returns descriptive metadata for the specified database.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11440-quandl.jpg
  humanURL: http://quandl.com
  baseURL: https://www.quandl.com//api/v3
  tags: Finance, Data, Finance, Target, Imports, Stack Network, internet, Technology,
    SaaS, Enterprise, Market Data, Sign In With Github, Sign In With Google, Sign
    In With LinkedIn, Have API Key, Visualizations, General Data, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/databasesdatabase-code-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/databasesdatabase-code-get-openapi.md
- name: Quandl - Get Databases
  x-api-slug: databases-get
  description: 'You can search for specific databases on Quandl by making the following
    API request.  The API will return databases related to your query. Databases are
    returned 100 results at a time. You can page through the results using these parameters:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11440-quandl.jpg
  humanURL: http://quandl.com
  baseURL: https://www.quandl.com//api/v3
  tags: Finance, Data, Finance, Target, Imports, Stack Network, internet, Technology,
    SaaS, Enterprise, Market Data, Sign In With Github, Sign In With Google, Sign
    In With LinkedIn, Have API Key, Visualizations, General Data, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/databases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quandl/master/_listings/quandl/databases-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://qualpay.api.gallery.streamdata.io
- type: x-api-stack
  url: http://quandl.stack.network
- type: x-authentication
  url: https://docs.quandl.com/docs#section-authentication
- type: x-blog
  url: http://blog.quandl.com/
- type: x-blog-rss
  url: http://blog.quandl.com/feed/
- type: x-branding
  url: https://www.quandl.com/brand-guidelines
- type: x-contact-form
  url: https://www.quandl.com/contact
- type: x-crunchbase
  url: https://crunchbase.com/organization/quandl
- type: x-documentation
  url: https://docs.quandl.com/
- type: x-errors
  url: https://docs.quandl.com/docs/error-codes
- type: x-getting-started
  url: https://docs.quandl.com/docs/getting-started
- type: x-linkedin
  url: https://www.linkedin.com/company/2459204/?trk=tyah&trkInfo=clickedVertical%3Acompany%2CclickedEntityId%3A2459204%2Cidx%3A2-1-2%2CtarId%3A1479320490204%2Ctas%3Aquandl
- type: x-login
  url: https://www.quandl.com/?modal=login
- type: x-press
  url: https://www.quandl.com/press
- type: x-spreadsheets
  url: https://docs.quandl.com/docs/excel-add-in
- type: x-status
  url: http://status.quandl.com/
- type: x-support
  url: https://docs.quandl.com/docs/contact-support
- type: x-terms-of-service
  url: https://www.quandl.com/terms
- type: x-twitter
  url: https://twitter.com/quandl
- type: x-website
  url: http://quandl.com
- type: x-website
  url: https://www.quandl.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---