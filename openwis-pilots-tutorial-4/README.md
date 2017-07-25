## OWT-4: Exposing a service via REST in Karaf using CXF
Apache CXF is an open source services framework that allows developers to build services using frontend programming APIs, like JAX-WS and JAX-RS. These services can speak a variety of protocols such as SOAP, XML/HTTP, RESTful HTTP, or CORBA and work over a variety of transports such as HTTP, JMS or JBI.

This tutorial will integrate CXF into OWT-3 and demonstrate the way to create a REST service using the framework.
The created service will contain 3 methods that will allow a client (e.g. browser) to:
1. Perform a GET request
2. Perform a POST request
3. Receive a response with a custom HTTP status code
