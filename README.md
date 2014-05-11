secret-octo-happiness
=====================

What is this?
-------------

Secret octo happiness is just a test project for Django-rest-framework `pip install djangorestframework`. 

It's pretty awesome. 

Snippets API
============

API Endpoint
------------

127.0.0.1:8000/api/snippets/

Headers


| Name | Value |
| ------------- | ------------- |
| Content-Type  | application/json  |
| Content-Type  | text/html  |


Usage
-----

A quick overview on how this test api works.

Get All Snippets
----------------

```
/api/snippets/
```

Sample Response JSON
--------------------
HTTP 200 OK
Content-Type: application/json
Vary: Accept
Allow: POST, OPTIONS, GET

```JSON

[
    {
        "pk": 1, 
        "title": "Epic Python", 
        "code": "oh boy you are in for it now", 
        "linenos": false, 
        "language": "python", 
        "style": "friendly"
    }, 
    {
        "pk": 2, 
        "title": "Some more Epic Python", 
        "code": "oh boy you are in for it now", 
        "linenos": false, 
        "language": "python", 
        "style": "friendly"
    }
]
```
