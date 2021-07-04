# Readings: Authentication


## what is basic access authentication?
- a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.

> Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know
<br/>
<br/>


## Authentication General Guidelines


a. Make sure your usernames/user IDs are
case-insensitive.
b. Usernames should also be unique.


<br/>

## Implement Proper Password Strength Controls

1. Minimum length of the passwords should be enforced by the application. Passwords shorter than 8 characters are considered to be weak.
 
2. Maximum password length should not be set too low, as it will prevent users from creating passphrases. A common maximum length is 64.


<br/>
<br/>

## what is node.bcrypt.js? 
- A library to help you hash passwords.

> npm install bcrypt


<br/>
<br/>







## Review, Research, and Discussion

1. Explain what a “Singleton” is (in Computer Science terms)

- A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object.
<br/>
<br/>


2. Explain how the Singleton pattern can be used with Node modules, specifically with classes

- A singleton is intended to provide only one instance of itself while facilitating a global point of access. Implementing a singleton pattern involves creating a class with a method that creates a new instance of the class. In order to implement a singleton pattern, principles of single instance and global access must be satisfied. The singleton class is like a global repository for an instance of itself, making the constructor private. Therefore, an instance outside the class cannot be created at all, and a singleton can contain only one instance. A singleton class instantiates itself and maintains that instance across systems.
<br/>
<br/>

3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

- Application Level Middleware

- Auth middleware

- Suppose we are having five routes getUsers,getDetails,updateDetails,isLoggedIn,isLoggedOut

- A middleware is basically a function that will the receive the Request and Response objects, just like your route Handlers do. As a third argument you have another function which you should call once your middleware code completed. This means you can wait for asynchronous database or network operations to finish before proceeding to the next


<br/>
<br/>

 ## Document the following Vocabulary Terms

### Term
1. Router Middleware

2. Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router().

> var router = express.Router() Dynamic Module Loading

3. Singleton Pattern
- In software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one “single” instance. This is useful when exactly one object is needed to coordinate actions across the system

4. Mock Testing
- Mock testing is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules.




## Preview (Links to an external site.)

1. Which 3 things had you heard about previously and now have better clarity on?
- Mock Testing, Singleton Pattern, CRUD.
<br/>
<br/>

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- Username Passwords and authentication, how user specific data is retrieved and rendered, creating a CRUD app utilizing username and password.
<br/>
<br/>

3. What are you most excited about trying to implement or see how it works?
- Username Passwords and Authentication.

<br/>
<br/>
<br/>
<br/>

References:

1. [ Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)<br/>
2. [Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)<br/>
3. [OWASP auth cheatsheet](https://www.owasp.org/index.php/Authentication_Cheat_Sheet)<br/>

4. [bcrypt docs](https://www.npmjs.com/package/bcrypt)


