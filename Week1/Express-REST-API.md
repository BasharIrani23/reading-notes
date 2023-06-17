# Express REST API
## ES 6 review
1- Classes are a template for creating ____.
 Classes are a template for creating objects.
 
2-Can a class declaration be hoisted?
- No, class declarations cannot be hoisted in most programming languages.
- 
3-How would you describe a constructor and contextual “this” to a non-technical friend?
- A constructor is a special method which will run when the class is automatically called when an object is created. 

## Using Express Routing 

1- Within Express, what does routing refer to?
- In Express, routing refers to how an application’s endpoints (URIs) respond to client requests.

2- What is the difference between a route path and a route method?
The route path determines the URL pattern to match, while the route method specifies the HTTP method to match.

3- When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?

we use next when we need to do a specific operation inside route handler and then pass control to the next one
We must call it to pass control to the next handler ,also to make sure that the application is working normally

## Express Routing
1-What is an Express Router?
An Express Router is a module in Express.js that helps organize and handle routes for HTTP requests.

2-By what mean do we initialize express.Router() in an express server?
import the Express module in server file , then create an instance of the Express Router using the express.Router() method.

3-What do we use route middleware for?
Route middleware is used to perform additional operations on specific routes. It can be used for tasks such as authentication, input validation, logging, etc.


## Reflection
- What are your learning goals after reading and reviewing the class README?
 I am interested in learning more about Express


