# Read: Class 13 - Readings: CRUD


## 1. In your own words, describe what each group of status code represents:

- 100’s = informational status codes. [using different protocol , request failure before even sending the body]

- 200’s = the success codes.[request accepted, if its an async func then that mean the request met all the requirements and not necessarily successful ]

- 300’s = redirection codes.[resources aren't available ]

- 400’s = client error codes.[invalid request from the client's end]  

- 500’s =server error codes.[overwhelmed servers or unreachable proxies.] 
    
<p>&nbsp;</p>

 ## 2. What is a status code 202?
 - 202 Accepted is used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future.
<p>&nbsp;</p>


 ## 3. What is a status code 308?
 - 308 Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore.
 <p>&nbsp;</p>


 ## 4. What code would you use if an update didn’t return data to a client?
 - 204 No Content - A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.
<p>&nbsp;</p>


 ## 5. What code would you use if a resource used to exist but no longer does?
 - 410 Gone - This is like 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.
 <p>&nbsp;</p>



 ## 6. What is the ‘Forbidden’ status code?
 - 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>

## What is the difference between PUT and PATCH?
- PUT will update the whole document but PATCH will update that specific document detail.

# References:
1. [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)
2. [Build A REST API With Node.js, Express, & MongoDB - Quick ](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)