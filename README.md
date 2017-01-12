interana-sdk Readme
============

This will contain a simplified SDK to enable easy access to the Interana APIs.
Being provided at a best-effort basis. So please use at your risk.

## High Level desciption of files

* **query_sdk\interana_client.py** - Python implementation of Interana SDK - Provides the Interana Object as a helper to query the Interana External API as documented [here](https://docs.interania.com/Guides/Reference/External_API%3A_query)

* **ingest_sdk** - TBD

* **ia_api_consumer.py** - Uses the Python SDK. Provides for further abstraction of the Interana Query API. Allows for easy access and validation to ensure that connectivity and results are as needed. Fork at will :)

## Usage

* Currently, the API Consumer utility only supports the Query APIs

* For the API Consumer script, there are three position parameters that need to be provided.
In addition, there are optional parameters that can be leveraged as well.

* To access Interana's Demo Cluster and do a simple count*, do:

`./ia_api_consumer.py tffZR6q0fbVqSBbeuvvLllLMLV0KHbuH+/DjXo9K=ER0PY/qNh+hdjEh+16DcL5Gc=BfHTJ7dE64x06YFWMbtbqtcdO90000 demo.interana.com music`

(note this will only work when you are on the Interana Corporate Network)

A sample output might look like this:

`$ ./ia_api_consumer.py tffZR6q0fbVqSBbeuvvLllLMLV0KHbuH+/DjXo9K=ER0PY/qNh+hdjEh+16DcL5Gc=BfHTJ7dE64x06YFWMbtbqtcdO90000 demo.interana.com music`

`-------------------------------------------`

`Results recieved from Interana:`

`-------------------------------------------`

`{u'rows': [{u'values': [[u'All'], 4058569848.0]}], u'columns': [{u'type': u'array', u'label': [u'result']}, {u'type': u'number', u'label': u'measure_value'}]}`

`-------------------------------------------`

`End of Results`

`-------------------------------------------`