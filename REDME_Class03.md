# DAY 2

## Question

**Name 3 real world use cases where you’d want to change the request with custom middleware ?**

*Authentcation*

*Data Management*

*Logging Middleware*

**True or false: The route handler is middleware?**

***false***

**In what ways can a middleware function end the process and send data to the browser?**

- res.send()
- res.render()
- res.end()
- res.json()

**At what point in the request lifecycle can you “inject” middleware?**

at any point after sending the request and before the response send(between them(middle))

**What can cause express to error with “Request headers sent twice, cannot start a second response” ?**

When we are in the finished state, but some function tried to set a statusCode.

## Vocabulary Terms

**Middleware** :  functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.

**Request Object** : The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.

**Response Object** : The res object represents the HTTP response that an Express app sends when it gets an HTTP request.

**Classes** : Are a template for creating objects. They encapsulate data with code to work on that data.

**Routing** : It is refers to how an application’s endpoints (URIs) respond to client requests.

**Routing Middleware** : It is a route which is using to log requests to the console or validate specific parameters If It is for parameters .

**Test Driven Development** : It is a programming practice which involves developing tests for every small functionality of an application.

**Behavioral Testing** : It is a testing of the external behavior of the program, also known as black box testing. It is usually a functional testing.

## Preview

**Which 3 things had you heard about previously and now have better clarity on?**
- Routing
- Request Object
- Response Object

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

- Middleware
- Test Driven Development
- Behavioral Testing

**What are you most excited about trying to implement or see how it works?**

- Middleware
