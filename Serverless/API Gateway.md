The API Gateway is a managed service that acts as an endpoint or entry point for apps and allows us to create and manage API. It can serve as a consistent front end in AWS and/or on-premises. 

It provides HTTP, REST or Websocket APIs. 

<img width="957" height="464" alt="Pasted image 20250726163956" src="https://github.com/user-attachments/assets/05f56d00-fc66-494a-80e7-d5fdf9dba0ae" />

### 1. Authentification 

API can be run with or without authentification .
Cognito is one of the services that is easily integrated for authentification. 

### 2. Endpoint Types

1. Edge-Optimized: routed to the nearest Cloudfront POP
2. Regional
3. Private: only within a VPC

### 3. Stages

APIs are deployed to stages which each have a deployment and an endpoint. Stages can be enabled for canary deployments. A small part will be used for testing and when ok, the canary will be promoted to make it the new base stage. 

### 4. Caching 

Caching (500MB to 237GB) is done on the stage level and allows for reduced load on the backend. 

<span class="red-text">Exam Tips: </span>

> 4XX ------> client side, invalid request 
> 5XX ------> server side, valid request
> 400 ------> Bad request 
> 403 ------> Access Denied
> 429 ------> throttling, amount of request exceeded
> 502 ------> Bad Gateway Exception - bad output returned by Lambda
> 503 ------> service unavailable
> 504 ------> Integration Failure / Timeout - 29s limit 

