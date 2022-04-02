# AWS: API, Dynamo and Lambda

**Amazon API Gateway**

Is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic

And its sits between the backend services of your API and your API’s users

***Benefits of Amazon API Gateway***

* Map HTTP requests to specific functions in a Serverless application via an API Gateway event

* Map WebSocket events to Serverless functions.

* Use multiple microservices to serve the same top-level API. 

* Save time with integrations: authentication, developer portal, CloudTrail, CloudWatch. 

![API](https://d2908q01vomqb2.cloudfront.net/1b6453892473a467d07372d45eb05abc2031647a/2018/06/13/api-backends.png)

Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale.

API Gateway handles all the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, CORS support, authorization and access control, throttling, monitoring, and API version management. 

**API Types**

* RESTful APIs
* WEBSOCKET APIs

![gateway](https://d1.awsstatic.com/serverless/New-API-GW-Diagram.c9fc9835d2a9aa00ef90d0ddc4c6402a2536de0d.png)

**DynamoDB**

Is a hosted NoSQL database offered by Amazon Web Services (AWS)

offers:

* reliable performance 
* a managed experience.
* a small, simple API allowing for simple key-value access

It designed to run high-performance applications at any scale. DynamoDB offers built-in security, continuous backups, automated multi-Region replication, in-memory caching, and data export tools. 

![DynamoDB](https://d1.awsstatic.com/product-marketing/DynamoDB/product-page-diagram_Amazon-DynamoDB.a8a97936b804de5abb83fec9329acd03dec33332.png)


**Dynamoose**

Dynamoose is a modeling tool for Amazon's DynamoDB.

**Key Features**

* Type safety
* High level API
* Easy to use syntax
* Ability to transform data before saving or retrieving documents
* Strict data modeling (validation, required attributes, and more)
* Support for DynamoDB Transactions
* Powerful Conditional/Filtering Support
* Callback & Promise support


[Home](../README.md)
