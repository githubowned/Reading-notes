# Readings: Express REST API

## Review, Research, and Discussion


1. Name 3 real world use cases where you’d want to change the request with custom middleware

1. Login authentication
2. Logging data to get user insights
3. Error handling
<br/>
<br/>

2. True or false: The route handler is middleware?
- False. A route handler can make requests and get responses without middleware. Middleware can be added to route handlers or other functions to alter/shape requests/responses.
<br/>
<br/>

3. In what ways can a middleware function end the process and send data to the browser?
- Through the use of the next() Or 500 errors. If an error is triggered, it will end the WRRC and send the 500 message to the user through the broswer.
<br/>
<br/>

4. At what point in the request lifecycle can you “inject” middleware?
- Middleware can be injected to shape the way the request object.

<br/>
<br/>

5. What can cause express to error with “Request headers sent twice, cannot start a second response”

- This happens when you have more than one response being sent to your client.

<br/>
<br/>
<br/>

## Document the following Vocabulary Terms

1. Middleware
- A software that lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications.
<br/>

2. Request Object
-  is one half of the request and response cycle to examine calls from the client side, make HTTP requests, and handle incoming data whether in a string or JSON object.
<br/>

3. Response Object
- is one half of the request and response cycle to send data from the server to the client-side through HTTP requests.
<br/>

4. Application Middleware 
- a middleware that is bound to an instance of express, using app.use() and app.VERB().
<br/>

5. Routing Middleware:  a middleware that bound to an instance of express.Router().
<br/>

6. Test Driven Development
- Test-driven development (TDD) is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.
<br/>

7. Behavioral Testing:
- Behavioural Testing is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.

<br/>
<br/>
<br/>

## Preview
---

1. Which 3 things had you heard about previously and now have better clarity on?
- Routing
- middleware
- testing
<br/>

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- tests
- the definition of files in the labs we take( like the ___tests___ things)
- How to memorize all these codes.

<br/>

3. What are you most excited about trying to implement or see how it works?
- when we can see live things working i guess and how we can connect all that. It should be exciting!

<br/>
<br/>
<br/>
<br/>

## References
---

[1. Review: ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

[2. Using Express Routing](https://expressjs.com/en/guide/routing.html)

[3. Express Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)