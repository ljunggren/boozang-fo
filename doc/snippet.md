The BZ snippet
============

Run Boozang without installation
--------------------------------
The Boozang html snippet allows you to run the Boozang tool completely without a client-side installation, or browser extension. 

Installation
------------
To install the Boozang snippet first download it to your server. That can be done from the management UI at ai.boozang.com. The snippet is unique for every single project, so make sure not to get them mixed up. To activate your application for testing simply copy it to your application root. 

Renaming the fragment
---------------------
The fragment is called bz.html by default but can be renamed to anything. Sometimes you want to isolate different environments from each other for user access policy reason, but still have them in the same directory in your vrsioning system. In that case, you can name them bz-dev.html, bz-staging.html and bz-production.html. 

Locating your application root
------------------------------
Different applications have different application roots. In a standard html application it will be where the index.html is located. In a standard Angular application it will be where the html files are published, like the public/ directory. 

Launching the Boozang tool 
--------------------------
After isntallation you can launch the application without the need for the Chrome extension. Do this by accessing the fragemnt in a web browser like

http://myapplication.com/bz.html

or 

http://myapplication.com/my-renamed-fragment.html


Any tests that have been created using the Chrome extension will still be available, and it´s possible to go between running the tool using the html snippet and Chrome extension.

Cross-browser testing
---------------------
Using the BZ fragemnt the Boozang tool can now be open in a variety of browsers without the need for any other client install. Current browsers supported are Google Chrome, Firefox, Safari and Opera. We recommend that you use one primary browser for authoring the tests, then running them across the difference browsers. 

User credentials
-----------------------------
In a secure environment you can add your user credentials to the bz-fragment to avoid entering user credentials. One way to do it is to create a personalized copy of your bz-fragment

```yaml
cd webroot
cp bz.html bz-mats.html
```
and adding the user credentials the following way
```yaml
<DOCTYPE html><script type='text/javascript' src='//localhost:8000/ide?id=5a0478cd4f69270984c529a3'></script>
<script>
username="email@domain.com";
password="password";
</script>
```

This can be particularly useful when running cross-browser testing to avoind entering login credentials. 