# Read: Class 02
## Readings: Express


1. What’s the difference between PUT and PATCH?
- The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.




2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server
- [Postman](https://www.postman.com/).<br/>
- [Mocky.io](https://designer.mocky.io/).<br/>
- [Moockoon](https://designer.mocky.io/).

3. Compare and contrast Swagger and APIDoc.js  Which HTTP status codes should be sent with each type of (un)successful API call?





## Status codes for HTTP response

- Information answers (100-199)
- Responses to success (200-299)
- Retransfers (300-399)
- Errors in the client (400-499)
- Errors with the server (500-599)

<br/>

<br/>



## SOAP and REST
- SOAP (Simple Object Access Protocol) is a standards-based web services access protocol that has been around for a long time. Originally developed by Microsoft.

- REST (Representational State Transfer) is another standard, made in response to SOAP’s shortcomings. It seeks to fix the problems with SOAP and provide a simpler method of accessing web services.

- The Similarities While SOAP and REST share similarities over the HTTP protocol, SOAP is a more rigid set of messaging patterns than REST. The rules in SOAP are important because we can’t achieve any level of standardization without them. REST as an architecture style does not require processing and is naturally more flexible. Both SOAP and REST rely on well-established rules that everyone has agreed to abide by in the interest of exchanging information.


<br/>

<br/>


### Differences:

- for SOAP :Language, platform, and transport independent (REST requires use of HTTP).
for SOAP :Works well in distributed enterprise environments (REST assumes direct point-to-point communication).

- REST is more efficient (SOAP uses XML for all messages, REST can use smaller message formats).
REST is faster (no extensive processing required).
REST is closer to other web technologies in design philosophy.

<br/>


### Why we Use TDD:
- “code coverage” is a common approach to evidencing the use of TDD; while high coverage does not guarantee appropriate use of TDD, coverage below 80% is likely to indicate deficiencies in a team’s mastery of TDD.

- version control logs should show that test code is checked in each time product code is checked in, in roughly comparable amounts.

<br/>
<br/>

### CD and CI
- ontinuous integration(CI) is a coding philosophy and set of practices that drive development teams to implement small changes and check in code to version control repositories frequently. Because most modern applications require developing code in different platforms and tools, the team needs a mechanism to integrate and validate its changes.

<br/>
<br/>
<br/>

# References:

1. [An introduction to NodeJS and Express](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)<br/>
2. [What is NPM?](https://docs.npmjs.com/getting-started/what-is-npm)<br/>
3. [What is TDD?](https://www.agilealliance.org/glossary/tdd/)<br/>
4. [CI/CD](https://www.youtube.com/watch?v=xSv_m3KhUO8) <br/>