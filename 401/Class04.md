# Readings: Data Modeling

## Review, Research, and Discussion
---

1. Name 3 advantages to Test Driven Development
      1. Better program design and higher code quality
      2. Detailed project documentation
      3. TDD reduces the time required for project development
      4. Code flexibility and easier maintenance





<br/>
<br/>


2. In what case would you need to use beforeEach() or afterEach() in a test suite?
      1. in an instance where tests should be explicit
      2. when tests should never share the same state between tests
<br/>
<br/>

3. What is one downside of Test Driven Development
- Probably, the strongest argument against TDD is that the tests need to be maintained because the code has got to. Whenever requirements change, you would like to vary the code and tests.
<br/>
<br/>

4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
- The most important difference between class and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.


- A child of an ES6 class is another type definition which extends the parent with new properties and methods, which in turn can be instantiated at runtime. A child of a prototype is another object instance which delegates to the parent any properties that aren’t implemented on the child.

- A class constructor creates an instance of the class. A constructor in JavaScript is just a plain old function that returns an object. The only thing special about a JavaScript constructor is that, when invoked with the new keyword, it assigns its prototype as the prototype of the returned object.

<br/>
<br/>


5. Why REST?
      1. Easy to Learn and Implement
      2. Scalability
      3. Cacheable
      4. Flexibility and Portability

<br/>
<br/>



## Document the following Vocabulary Terms
---

## functional programming
- functional programming is a programming paradigm where programs are constructed by applying and composing functions.

## object-oriented programming (OOP)
- Object-oriented programming is a programming paradigm based on the concept of "objects", which can contain data and code: data in the form of fields, and code, in the form of procedures. A feature of objects is that an object's own procedures can access and often modify the data fields of itself. 

## class
-  A class is a blueprint that defines the variables and the methods common to all objects of a certain kind.

## super
- the parent class of the derived one.

## this
- pointer to the current object you are using.

## Test Driven Development (TDD)
- is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.

## Jest
- is a JavaScript testing framework maintained by Facebook, Inc.

## Continuous Integration (CI)
- is a software development practice in which developers merge their changes to the main branch many times per day.

## REST
- a software architectural style which uses a subset of HTTP. It is commonly used to create interactive applications that use Web services. Data Model: is an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities

## Data Model
- A data model refers to the logical inter-relationships and data flow between different data elements involved in the information world. It also documents the way data is stored and retrieved. … Data models help represent what data is required and what format is to be used for different business processes

<br/>
<br/>

## Preview
---

1. Which 3 things had you heard about previously and now have better clarity on?
- none so far.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- mostly testing with the new router method (thats all).

3. What are you most excited about trying to implement or see how it works?
- using a live API.
<br/>
<br/>
<br/>
<br/>

# References:

1. [sql vs nosql ](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)<br/>
2. [nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)<br/>
3. [nosql modeling techniques](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/)<br/>
4. [mongoose api](https://mongoosejs.com/docs/api.html#Model) <br/>
5. [What is TDD?](https://www.codica.com/blog/test-driven-development-benefits/)<br/>
