# intro-to-serverless
> An introduction to Serverless Framework

## Agenda

- Introduction to Serverless Architecture
- Introduction to Open-Source Serverless Framework
  - Quickstart
  - Language Support
  - Services
  - Extending Serverless Framework with [plugins](https://github.com/serverless/plugins)
  - [Serverless Framework Components](https://github.com/serverless-components)
- Build a Live Demo
- Use Cases
- Key concepts and taking from dev to production
- Discussions/Wrap-up

### Introduction to Serverless Architecture

- Microservice-y architecture for which you don't have to manage the infrastructure
- Infrastructure often abstracted away into simple configuration by Cloud Providers (AWS Lambda, Azure functions, Google CloudFunctions, etc.) or your in-house infrastructure team (With deployment of Apache OpenWhisk, Kubeless, Fission, etc.)
- Lowers the total cost of maintaining your apps, enabling you to build more logic, faster

### Introduction to Open-Source Serverless Framework

- MIT open-source project, actively maintained by a full-time, venture-backed team
- Supports Node.js, Python, Java, Go, C#, Ruby, Swift, Kotlin, PHP, Scala, & F#
- Manages the lifecycle of your serverless architecture (build, deploy, update, delete)
- Safely deploy functions, events and their required resources together via provider resource managers (e.g., AWS CloudFormation).
- Infrastructure abstraction sounds nice in theory, in practice, managing layers on top of that abstraction in a simple and unified way becomes fragile and so comes serverless framework for the rescue.
- Easy scaffolding, built-in support for stages, functions group (aka serverless services), easy to build CI/CD workflows and extensible via plugin system. Finally a big community

#### Quickstart

- `npm install -g serverless` or `curl -o- -L https://slss.io/install | bash`
- `serverless` or `sls` for running serverless
- `sls create -t aws-nodejs -p <app_name>`
- serverless.yml for configuration
