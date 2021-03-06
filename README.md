Overview
==========

This will contain a simplified SDK to enable easy access to the Interana APIs.
Being provided at a best-effort basis. So please use at your risk.

High Level desciption of files
==============================

TBD

Install
=======

Python SDK 

This can be installed by using pip directly. Dependencies will be installed automatically.

```pip install interanasdk```

This installs a python module called interanasdk and also, a command line script which allows for easy access to the SDK.

R SDK

TBD

Usage
=====

* To access the Python SDK in code, do the following:
```
/usr/bin/env python
import interanasdk
```

* To access the IA Query Client script, there are three positional parameters that need to be provided.
In addition, there are optional parameters that can be leveraged as well.

* To access Interana's Demo Cluster and do a simple count*, do:

```
ia_query_client tffZR6q0fbVqSBbeuvvLllLMLV0KHbuH+/DjXo9K=ER0PY/qNh+hdjEh+16DcL5Gc=BfHTJ7dE64x06YFWMbtbqtcdO90000 demo2.interana.com music
```

(note this will only work when you are on the Interana Corporate Network)

A sample output might look like this:

```
$ ia_query_client.py tffZR6q0fbVqSBbeuvvLllLMLV0KHbuH+/DjXo9K=ER0PY/qNh+hdjEh+16DcL5Gc=BfHTJ7dE64x06YFWMbtbqtcdO90000 demo2.interana.com music
-------------------------------------------
Results recieved from Interana:
-------------------------------------------
{u'rows': [{u'values': [[u'All'], 4058569848.0]}], u'columns': [{u'type': u'array', u'label': [u'result']}, {u'type': u'number', u'label': u'measure_value'}]}
-------------------------------------------
End of Results
-------------------------------------------
```

How to Contribute
==================
Simple. Feel free to jump in and contribute code. Some of the immediate next steps are:
* R implementation - work in progress
* MS-Excel (Windows only) implementation
* Jupyter Notebook
* Perl Implementation

Support & License
=======
## Support
The SDK is provided on a best-effort basis only. All support will be community-driven only.

## License
We have adopted the MIT license (see the file LICENSE.txt) for this project.
