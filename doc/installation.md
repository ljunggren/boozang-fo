Installation
============

Installation Options
------------
Boozang is completely hosted in the Cloud so there is no need for a client-side installation. Simply create a project and download the bz.html snippet and put it into your web application root. For users who do not have access to the application root we also provide a Chrome browser extension. This extension also allows for cross-domain testing which the html-snippet technology does not allow.

HTML snippet
---------------
The html snippet technology is completely secure as it´s reliant on the built-in security of the HTTP protocol. Simply create a project at http://ai.boozang.com and download the html snippet. The snippet is copied to the web root (where your index.html or similar would be located). In order to launch the Boozang tool, simply access the snippet in any browser, such as http://myapplication.com/bz.html or http://localhost:8080/bz.html. 

Chrome extension
---------------
For users without access to the application web root, or for users who wants to do cross-domain testing, we also provide a Chrome extension. The Chrome extension can be downloaded from the Chrome web store here: https://chrome.google.com/webstore/detail/boozang/feijjbehfljebjillfefcehfmlolcomf

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

Npm package for CI integration
-----------------------------
We also provide a npm package based on the excellent Headless Chrome Node API  Puppeteer, provided by Google developers (https://github.com/GoogleChrome/puppeteer). Install Node v8 or later and run 

```yaml
npm install boozang
```
This will automatically download a Chromium version compatible with your system that allows for headless execution. You can run any tests by specifying the URL of the test 

```yaml
boozang http://myapplication.com/bz.html#ost
```
