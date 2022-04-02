# AWS: API, Dynamo and Lambda

## AWS API Gateway Overview
Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

## How does API Gateway work?
API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services.

## AWS API Gateway 
The Amazon API Gateway service is a fully managed service that allows developers to easily construct, publish, maintain, monitor, and protect APIs at any size. APIs allow applications to access data, business logic, and functionality from your backend services through a “front door.” RESTful APIs and WebSocket APIs can be created with API Gateway to enable real-time two-way communication applications. Web applications, as well as containerized and serverless workloads, are supported by API Gateway.

API Gateway handles traffic management, CORS support, authorization and access control, throttling, monitoring, and API version management, as well as other responsibilities involved in accepting and processing hundreds of thousands of concurrent API calls. There are no minimum fees or initial costs with API Gateway. You pay for the API calls you receive and the data you send out, and you can save money by using the API Gateway’s tiered pricing model as your API usage grows.

## API Types 
- RESTful APIs
- WEBSOCKET APIs


## AWS DynamoDB Guide 
### What is DynamoDB?

Amazon Web Services’ DynamoDB is a hosted NoSQL database (AWS.It has the following features:

1. Consistent performance as the system grows.
2. a managed experience, which eliminates the need to SSH into servers to upgrade crypto libraries.
3. a modest, straightforward API that allows for basic key-value access as well as more complex query patterns.

**DynamoDB is especially well-suited to the following scenarios:**

1. Data-intensive applications with strict latency constraints. JOINs and complex SQL operations might slow down your queries as the amount of data you have grows. Your queries will have predictable latency using DynamoDB, even if they are large, up to 100 TBs!

2. AWS Lambda-based serverless applications. In reaction to event triggers, AWS Lambda provides auto-scaling, stateless, ephemeral compute. DynamoDB is a wonderful fit for constructing Serverless applications because it has an HTTP API and uses IAM roles for authentication and permission.

3. Data sets having well-known and easy access patterns. DynamoDB’s straightforward key-value access patterns make it a fast and reliable solution for creating and serving recommendations to users.

### AWS DynamoDB 
Fast, flexible NoSQL database service for single-digit millisecond performance at any scale

How it works Amazon DynamoDB is a serverless, fully managed key-value NoSQL database built to run high-performance applications at any size. Built-in security, continuous backups, automated multi-Region replication, in-memory cache, and data export tools are all features of DynamoDB.

## Dynamoose
is a modeling tool for Amazon's DynamoDB.

Key Features

- Type safety
- High level API
- Easy to use syntax
- Ability to transform data before saving or retrieving documents
- Strict data modeling (validation, required attributes, and more)
- Support for DynamoDB Transactions
- Powerful Conditional/Filtering Support
- Callback & Promise support