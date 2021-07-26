# Read 33: Authentication & Production Server

### What is JSON Web Token?
JSON Web Tokens are a useful tool and a better way of implementing authorization in web applications, but what exactly are they and how do they work?

What is a JWT? A JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

A JWT is a means of representing claims to be transferred between two parties. The claims in a JWT are encoded as a JSON object that is digitally signed using JSON Web Signature (JWS) and/or encrypted using JSON Web Encryption (JWE).


## When should you use JSON Web Tokens?

•Authorization: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. 

•Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. 


## How JWT Works (JSON Web Token)?

The JWT is just an authorization token that should be included in all requests 
its acquired by exchanging an username + password for an access token and an refresh token.

The access token is usually short-lived (expires in 5 min or so, can be customized though).

The refresh token lives a little bit longer (expires in 24 hours, also customizable). It is comparable to an authentication session. After it expires, you need a full login with username + password again.

### Those are three distinctive parts that compose a JWT:

• header

• payload 

• signature

## Django Runserver 

A production setup usually consists of multiple components, each designed and built to be really good at one specific thing. They are fast, reliable and very focused.

When a request arrives at your server, it should be passed to a dedicated web server. Nginx is an example for a good web server.

This is an application, which is great at serving static files from disk (your css and js files for example) and handling multiple requests at once. If the request is not for a static file, but should be processed by your application, the webserver is configured to pass this request to the next component.

The next component is an application server.
It gets those fancy requests and uses them to construct Python objects which are usable by Django. WSGI is a specification which people agreed on, which describe how that happens. Gunicorn is an example for a WSGI server.

