Validation
============

Useful resources
----------------
In order to simply mockup a REST server we strongly recommend https://github.com/typicode/json-server that allows you to create a fake REST API from a JSON file in less than 30 seconds. 


Creating a simple API validation
----------------------------
The API validation is very similar to a HTML validation except that the validation is done towards an API end-point.  

Validate Exists
---------------
The default validation is "Validate Exists", that will simple verify that the element exists. To edit the validation simply change it from the action detail page.  


Inner Text
----------
If you want to validate the content of an element, change the Content format dropdown to innerText. This way the text content of an element is compared. When changing this, the result box will be populated with the content from your application, but can be changed manually. 

Data
----
The data format is very powerful, but TODO

Screenshot
----------
You can also choose to take a picture of the element and compare that to the image of an element of future runs. This is useful TODO

The DOM picker
--------------
Sometimes the element you selected in the page isn't the one you intended. In this case, simply click the DOM picker and re-select the element. The DOM picker dialog will popup where you can select exactly what to validate in the DOM tree. Use the checkboxes to select which elements to include in the matching. Make sure that the checkbox has a green highlight, which means the element is uniquely matched (not indexed).