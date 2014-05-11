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

Attributes

| Name | Value |
| ------------- | ------------- |
| Content-Type  | application/json  |

Usage
-----

A quick overview on how this test api works.

Get All Snippets
----------------

```
/api/snippets/
```


Attributes

| Name | Value |
| ------------- | ------------- |
| Method  | Get |


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

Get Snippet
-----------

```
/api/snippets/<id>/
```

Returns ID specific snippet


Attributes

| Name | Value |
| ------------- | ------------- |
| Content-Type  | application/json  |
| Method  | Get |

Example
-------
```
/api/snippets/2/
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
        "pk": 2, 
        "title": "Some more Epic Python", 
        "code": "oh boy you are in for it now", 
        "linenos": false, 
        "language": "python", 
        "style": "friendly"
    }
]

Add Snippet
-----------

```
/api/snippets/
```

Posts a new Snippet


Attributes

| Name | Value |
| ------------- | ------------- |
| Content-Type  | application/json  |
| Method  | POST |

Example
-------
```
/api/snippets/2/
```

Sample Request JSON
--------------------

```JSON
[ 
    {
        "pk": 3, 
        "title": "Even more Epic Python", 
        "code": "oh boy you are in for it now", 
        "linenos": false, 
        "language": "python", 
        "style": "friendly"
    }
]
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
        "pk": 2, 
        "title": "Some more Epic Python", 
        "code": "oh boy you are in for it now", 
        "linenos": false, 
        "language": "python", 
        "style": "friendly"
    }
]
```
