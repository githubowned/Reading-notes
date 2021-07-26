# Readings: AWS: API, Dynamo and Lambda

## What is Amazon API Gateway?
- Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

<br/>
<br/>


## Many AWS services support integration with Amazon API Gateway, including:

- AWS Lambda: run Lambda functions to generate HTTP API responses.
- AWS SNS: publish SNS notifications when an HTTP API endpoint is accessed.
- Amazon Cognito: provide authentication and authorization for your HTTP APIs.
<br/>
<br/>

## What is Dynamoose?
- DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS).
- Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.
<br/>
<br/>

 ## Key Features
- Type safety.
- High level API.
- Easy to use syntax.
- Ability to transform data before saving or - retrieving documents.
- Strict data modeling (validation, required attributes, and more).
- Support for DynamoDB Transactions..
- Powerful Conditional/Filtering Support..
- Callback & Promise support.

<br/>
<br/>
<br/>

## Review
1. What are serverless functions?
- A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. 
<br/>
<br/>

2. If you were to create a system that emulated 
 Lambda functions, how would you do it?

 - “Open the Functions page on the Lambda console.
Choose Create function.
Under Basic information, do the following:
For Function name, enter my-function.
For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell, C#), Go, Java, Node.js, Python, and Ruby.
Choose Create function.
Lambda creates a Node.js function and an execution role that grants the function permission to upload logs. The Lambda function assumes the execution role when you invoke your function, and uses the execution role to create credentials for the AWS SDK and to read data from event sources”.
<br/>
<br/>

3. Describe how a CDN works
- A CDN (Content Delivery Network) is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user. This helps users around the world view the same high-quality content without slow loading times.
<br/>

- Without a CDN, content origin servers must respond to every single end user request. This results in significant traffic to the origin and subsequent load, thereby increasing the chances for origin failure if the traffic spikes are exceedingly high or if the load is persistent.
<br/>

- By responding to end user requests in place of the origin and in closer physical and network proximity to the end user, a CDN offloads traffic from content servers and improves the web experience, thus benefiting both the content provider and its end users.
<br/>
<br/>

## Terms
- Serverless Functions: serverless functions are single-purpose, programmatic functions that are hosted on managed infrastructure. These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies. The engineering teams within those companies ensure that the serverless functions have near-perfect uptime, redundant instances around the world, and scale to any incoming network request volume.
<br/>

- Cloud Storage: Object storage for companies of all sizes. Store any amount of data.
<br/>

- CDN :  A content delivery network, or content distribution network (CDN), is a geographically distributed network of proxy servers and their data centers. The goal is to provide high availability and performance by distributing the service spatially relative to end users.


# preview

 Which 3 things had you heard about previously and now have better clarity on?
- AWS console.
<br/>
<br/>

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- lambda functions.
<br/>
<br/>

 What are you most excited about trying to implement or see how it works?
- CRUD on AWS.

<br/>
<br/>
<br/>
<br/>

# References
[AWS API Gateway Overview](https://www.serverless.com/amazon-api-gateway)

[AWS API Gateway](https://aws.amazon.com/api-gateway/)

[AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)

[AWS DynamoDB](https://aws.amazon.com/dynamodb/)

[Dynamoose](https://dynamoosejs.com/getting_started/Introduction)
