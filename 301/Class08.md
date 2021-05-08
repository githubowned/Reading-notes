# Read: Class 08 - Readings: APIs

## What does REST stand for?
- REST API : REST stands for Representational state transfer , which is a software architectural style which uses a subset of HTTP. It is commonly used to create interactive applications that use Web services. A Web service that follows these guidelines is called RESTful. REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client

<p>&nbsp;</p>

## What are the most common HTTP verbs?
- The most common operations are GET, POST, PUT, PATCH, and DELETE.

<p>&nbsp;</p>

## What should the URIs be based on?
- On nouns (the resource) and not verbs (the operations on the resource).

<p>&nbsp;</p>

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
- All web requests impose a load on the web server. The more requests, the bigger the load. Therefore, try to avoid “chatty” web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. 


- Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request. However, you need to balance this approach against the overhead of fetching data that the client doesn’t need. Retrieving large objects can increase the latency of a request and incur additional bandwidth costs.

<p>&nbsp;</p>

## What status code does a successful POST request return?
-
If a POST method creates a new resource, it returns HTTP status code 201 (Created). The URI of the new resource is included in the Location header of the response. The response body contains a representation of the resource. If the method does some processing but does not create a new resource, the method can return HTTP status code 200 and include the result of the operation in the response body.

<p>&nbsp;</p>

## What status code does a successful DELETE request return?
- The web server should respond with HTTP status code 204, indicating that the process has been successfully handled, but that the response body contains no further information.


<p>&nbsp;</p>





## References:
---

1. [API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)








