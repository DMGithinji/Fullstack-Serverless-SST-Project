# A Simple Serverless Stack (SST) Application.

AWS Lambda is a compute service that lets you run code without provisioning or managing servers. 

But working directly with AWS Lambda, API Gateway, and the other AWS services can be a bit cumbersome. Since these services run on AWS, it can be tricky to test and debug them locally.
Ideally, we wouldn’t want to have to click through the AWS Console to create our infrastructure, rather we would want our infrastructure to be created programmatically.

To solve these, there are solutions such as Serverless Stack Framework (SST) and Serverless Framework.

In this project, I work with [Serverless Stack Framework (sst)](https://docs.serverless-stack.com/packages/create-serverless-stack) to generate infrastructure code that describes Lambda functions, API Gateway endpoints, DynamoDB tables, S3 buckets.  SST converts the infra code into CloudFormation templates which enables resources to be provisioned based on that.
I'm then consuming the APIS using React frontend.



## Getting Started
Start by installing the dependencies.

```bash
$ npm install
```

## Commands

### `npm run start`

Starts the local Lambda development environment.

### `npm run build`

Build your app and synthesize your stacks.

Generates a `.build/` directory with the compiled files and a `.build/cdk.out/` directory with the synthesized CloudFormation stacks.

### `npm run deploy [stack]`

Deploy all your stacks to AWS. Or optionally deploy, a specific stack.

### `npm run remove [stack]`

Remove all your stacks and all of their resources from AWS. Or optionally removes, a specific stack.

### `npm run test`

Runs your tests using Jest. Takes all the [Jest CLI options](https://jestjs.io/docs/en/cli).

## Documentation

Learn more about the Serverless Stack.
- [Docs](https://docs.serverless-stack.com)
- [@serverless-stack/cli](https://docs.serverless-stack.com/packages/cli)
- [@serverless-stack/resources](https://docs.serverless-stack.com/packages/resources)
