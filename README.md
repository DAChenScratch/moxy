

`npm install`

`npm start`

The default prefix for Alloy Proxy will is "/proxy/" but you are free to change this in "config.json" alongside the port.

# How the proxy works:

The proxy works by using node-fetch (Basically Window.fetch ported to Node-js). 
Basically what the app is doing is node-fetch is sending the request to the server then
the app sends the response back to the server with the modifactions made to the attributes and elements.

When a attribute is rewritten, depending on the contents inside. It will turn:

`href="/assets/js/main.js"` into `href="/fetch/websiteURL/assets/js/main.js"`.

A porition of its rewriting is in client-side JS so `Element.setAttribute`, `window.fetch()`, XMLHttpRequest, and more are rewritten.

# Implementing your website in Alloyproxy

To implement your website into AlloyProxy. Upload all of your files into the `public` folder then your done.

# Blacklisting websites!

If you don't want certain websites such as porn websites to be accessed.
You can add a websites hostname to `blocklist.json`.
A websites hostname is the URL of a 
