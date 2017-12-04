Extracting data from an API
===========================

Similarities with Validation
---------------
Extracting data is identical to API validation except that the returned respons will be saved in a data variable. Make sure to familiarize yourself with the API Validation action before reading this section. 

Introducing data
----------------
Start by defining a data variable in the data tab. For extraction of API data you typically want to use an Object. The Object can be defined on project, module and test level. Add it on test level if the data will only be used in the test case. Add it on module level if the data will be used across different tests in the module, but not on different modules. Add it on project level if it will be used globally. 

Assigning data
--------------
The result will be contained in the $result variable. To assign the API response to test data called "dummy" write the following in the Extract Data window

$test.dummy = $result


Data Conversion
----------------



Extracting data action
----------------------
To add an extract data action, simply click on the Plus icon and select Extract data, then click on an element in the application window you want to extract. 
