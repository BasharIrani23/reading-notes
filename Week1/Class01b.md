# An introduction to NodeJS and Express

## 1-Explain middleware, answer as though I were a non-technical recruiter.
middleware is something falls between the functions and methods , 
usually it makes some operations on the requests and response , then it call the next functions on the order.

## 2-Express the most popular __ __ ____.
Express is the most popular Node web framework,

## 3-Express is “unopinionated.” What does that mean?

Opinionated frameworks are those with opinions about the "right way" to handle any particular task. They often support rapid development in a particular domain (solving problems of a particular type) because the right way to do anything is usually well-understood and well-documented
The oppoisite is the "unopinionated" , They make it easier for developers to use the most suitable tools to complete a particular task
and when we say Express in unopinionated , it means you can insert almost any compatible middleware you like into the request handling chain,
in almost any order you like. 
You can structure the app in one file or multiple files, and using any directory structure. You may sometimes feel that you have too many choices.

## 4-What is a module and why is modularity useful to us as developers?
A module is a JavaScript library/file that you can import into other code using Node's require() function.
module can break down a software system into smaller, modular units, developers can reuse these modules in different projects or parts of the same project
also modules can promotes collaboration among developers by dividing the development tasks into smaller
***
# What is NPM?
## 1- What version of npm are you running on your machine?
To check it , i have to type npm -v in my terminal , and the version is running on my device is **9.5.1**

## 2-What command would you type to install a library/package called ‘jshint’ into your node project?
**npm install jshint**
***

# What is TDD?
## 1-Explain why tests are important. Please explain as though I were your non technical elder.
In general , tests are safety nets or quality control measures for the software we develop.
#### why it is important ?
Tests help to ensure that the software works as intended and behaving correctly under different scenarios.

## 2-What are three expected benefits of testing
- Collaboration: Tests also help developers work together more effectively. When different people are working on the same project, tests provide a common language to understand and validate the software's behavior.
- Refactoring Confidence: Refactoring means making changes to the code without changing its external behavior. Tests give us the confidence to make these changes by providing a safety net.
- Preventing Mistakes: Tests can catch mistakes or errors in our code before they cause bigger problems.

## 3-Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.
#### Individual pitfalls 
- Forgetting to run tests frequently
- Writing too many tests at once
- Writing tests that are too large or coarse-grained
#### Team pitfalls
- Partial adoption
- Poor maintenance of the test suite
- Abandoned test suite
*** 
# CI/CD
## 1- What are three benefits of Continuous Integration?
- Reduced Integration Problems
- Increase Code Confidence
- Early Detection of Issues
## 2-What is the difference between Continuos Delivery and Continuous Deployment?
While they are similar in concept, there is a key difference between the them 
The Automation deploy of the production , the **CDep** allowing software changes to be automatically deployed to production without manual intervention.
on the other hand , the  decision of when to release the software to production in the **CD** is made manually by the development team or stakeholders.

## 3-Explain how GitHub fits into this process assuming the listener comes from a non-technical background
GitHub serves as a collaboration platform. Allows developers to integrate their work, test and deploy software.

# Reflection
### What are your learning goals after reading and reviewing the class README?
Describe and Define
- Node Modules
- Code Modularization
- Express Middleware
- HTTP Status Codes
- TDD and Testing
- Write an express API server
- Incorporate application level middleware
- Properly test an express server
