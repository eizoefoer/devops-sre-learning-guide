# Serverless and API's 101

## RESTful API's

#### REST links

- [Best Practices for Designing a Pragmatic RESTful API](https://www.vinaysahni.com/best-practices-for-a-pragmatic-restful-api)
- Swagger/OpenAPI
  - [What is Swagger?](https://swagger.io/docs/specification/2-0/what-is-swagger/)
  - [Swagger UI Editor](https://editor.swagger.io/)

## Serverless

Serverless is a technical and monetary abstraction of resources running on a public Cloud Provider such as AWS, Azure, GCP.
- **Technical**: Underlying infrastructure is managed for you by your Cloud Provider and hidden from you (you can't see or touch it!). As an example for AWS Lambda, it runs on EC2 instances but you don't have to provision and manage your Virtual Machines. 
- **Monetary**: You pay for the serverless resource and not the things your Cloud Provider runs it on. Often an on-demand and pay-per-use model.

#### Pros

- You don't have to manage the Virtual Machines, Scaling, etc
- It "can" be cheaper with a pay-per-use model.

#### Cons

- You have less control of the underlying infrastructure. I.E You cannot configure your storage, network, security, CPU and memory to the same extent as a standard resource. Examples:
  - AWS Lambda network bandwidth and CPU scales with allocated memory.
  - You cannot mount volumes to AWS Lambda
  - AWS Fargate does not support EFS
- Many Serverless resources are Cloud vendor-specific, i.e Not Cloud Agnostic.
- The pay-per-use model will be more expensive if it is running inefficiently. Running an ECS container on an EC2 Instance 24/7 will be much than running a Serverless ECS Fargate task 24/7. 

#### Serverless vs Managed Service Examples

Cloud providers also have "Managed Services". These are not Serverless. Although they may be hidden from you (i.e can't see the EC2 Instances) you still are billed for the underlying infrastructure resources and it is not pay-per-use.

**Serverless examples**: AWS Lambda, API Gateway, DynamoDB, SQS, SNS, Fargate, Glue, etc...

**Managed Services example**: AWS Elasticsearch, RDS (excluding Aurora Serverless), Amazon DocumentDB, EMR, etc...

  - Correct: You pay for AWS Lambda resources and not the EC2 instances it runs on.
  - Incorrect: AWS Elasticsearch your bill displays EC2, EBS, etc... This is not Serverless, but an AWS Managed Service!!!

#### 101 Links

- [AWS Serverless](https://aws.amazon.com/serverless/)
- [Serverless Patterns](https://serverlesspatterns.io/)

#### Advanced Links
- [Amazon DynamoDB deep dive: Advanced design patterns](https://www.youtube.com/watch?v=6yqfmXiZTlM)
- 
- [AWS Lambda under the hood](https://www.youtube.com/watch?v=xmacMfbrG28)
- [AWS Fargate under the hood](https://www.youtube.com/watch?v=Hr-zOaBGyEA)

#### AWS SAM

An extension of AWS CloudFormation (Infrastructure-as-Code) that specialises in Serverless and Events.

**Repos and Guides**
- [AWS SAM Github](https://github.com/awslabs/serverless-application-model)
- [AWS SAM Examples](https://github.com/awslabs/serverless-application-model/tree/develop/examples/2016-10-31)

**Tutorials and Workshops**
- [AWS Serverless Workshops](https://github.com/aws-samples/aws-serverless-workshops)

**Live Coding Demo Videos**
- [AWS Build on Serverless Playlist](https://www.youtube.com/playlist?list=PLhr1KZpdzukcYWC1xD-vidMZf2uilGkor)
- [AWS Serverless: Happy Little APIs](https://www.youtube.com/playlist?list=PLhr1KZpdzukfphWGOWYOJSNhPe9PhM_1z)

**AWS SAM Deep Dive Videos**
- [Deep Dive into AWS SAM](https://www.youtube.com/watch?v=CIdUU6rNdk4)
- [An in-depth tour of AWS SAM](https://www.youtube.com/watch?v=VG_nEWsiiGw)
- [AWS SAM toolkit: Build, test & debug your serverless applications](https://www.youtube.com/watch?v=3gCzGLdhQao)

**AWS Serverless API Videos**
- [I didn’t know Amazon API Gateway did that](https://www.youtube.com/watch?v=yfJZc3sJZ8E)
- [Building APIs from front to back](https://www.youtube.com/watch?v=cc_pKfDOH2E)

#### Serverless RESTful API Frameworks

Frameworks that are structured like traditional Web/API Frameworks (Django, Flask, Rails, Express, etc...). Use this if you don't want to use Infrastructure-as-Code style videos.

- [The "Serverless Framework" (NodeJS)](https://serverless.com/)
- [Zappa (Python with Django and Flask Support)](https://github.com/Miserlou/Zappa)
- [Chalice (Python, made by AWS)](https://github.com/aws/chalice)
