# AWS: API, Dynamo and Lambda
## AWS API Gateway Overview
### 1.What is Amazon API Gateway?
AWS offers a service that enables programmers to build, publish, maintain, watch, and secure APIs at any scale.

### 2.Why is Amazon API Gateway an important part of the Serverless ecosystem?
It serves as the starting point for serverless applications and makes it simple to integrate serverless functions (AWS Lambda) with other services.

### 3.How does API Gateway integrate with other AWS services?
It can interface with Amazon S3 Links to an external website and directly connect to AWS Lambda functions to run backend functionality.
***
## AWS API Gateway
1.What are the some benefits of using Amazon API Gateway?
- Simple API creation and administration.
- ability to scale to accommodate any volume of incoming traffic.
2.What two API types might you choose from?
REST APIs
WebSocket APIs
***
## AWS DynamoDB Guide
### 1.What is DynamoDB?
AWS offers a service for NoSQL databases
For applications requiring flexible data models, it offers high availability and minimal latency.

### 2.Under what circumstances would you recommend DynamoDB over MongoDB?
If you want to avoid managing infrastructure and need automatic scaling, then yes. 
***
## AWS DynamoDB
### 1.Explain to a non-technical friend how DynamoDB works.

Data is stored and retrieved through DynamoDB, an AWS database service. Similar to a digital table, you can store information there and readily access it later.
Links leading to other websites.Dynamoose
***
## Dynamoose
### 1-What is Dynamoose?
an npm package that provides an easier way to work with DynamoDB in Node.js applications.
### 2-What are some key features of Dynamoose?
- Models and schemas can be defined using a simpler syntax.
- support for type checking and data validation.
- Async/await integration enables more fluid asynchronous processes.
