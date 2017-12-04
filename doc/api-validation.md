Validation of API end-points
============

Useful resources
----------------
In order to simply mockup a REST server we strongly recommend https://github.com/typicode/json-server that allows you to create a fake REST API from a JSON file in less than 30 seconds. 


Introduction to API validations
-------------------------------
The API validation is very similar to a HTML validation except that the validation is done towards an API end-point. Simply click on the Plus-sign and choose "Validation", and select Request/Response (API). In actions details you can now input the API end-point URL and HTTP method (GET, POST, DELETE, etc.).

Doing HTTP GET validation
-------------------------
Use HTTP method GET to validate a response from a REST API. Simply select HTTP method GET and enter the end-point URL. Click Play on the action to automatically populate the expectation value. 

Doing a HTTP GET without validation
-----------------------------------
In order to trigger the HTTP GET without validating the result simply use comparison operator to "regexp" and set the expectation field to ".*". 

Adding custom headers
---------------------
When doing API calls it's very common that you need to add custom HTTP request headers. In order to do this click HTTP headers and add header data. This needs to be in data format, i.e.

{
  Accept:"json"
}

Doing HTTP POST validation
--------------------------
You can post data to an API end-pont using HTTP method POST. When doing thi make sure to add the POST data to the HTTP data field. 

Data
----
In all these fields you can also bind data. As an example, in order to set headers as data this can be done as an object, for instance "jsonheader","Accept","json". In order to reference it on the actions details use {{$test.jsonheader}} in the header field. 