# CDK API Gateway and Lambda sample

Template for deploying API Gateway and Lambda functions using AWS CDK

## Constructs and constructors

1. scope: the first argument is always the scope in which this construct is created. In almost all cases, you'll be defining constructs within the scope of current construct, which means you'll usually just want to pass this for the first argument. Make a habit out of it.
2. id: the second argument is the local identity of the construct. It's an ID that has to be unique amongst construct within the same scope. The CDK uses this identity to calculate the CloudFormation Logical ID
   for each resource defined within this scope. To read more about IDs in the CDK, see the CDK user manual.
3. props: the last (sometimes optional) argument is always a set of initialization properties. Those are specific to each construct. For example, the lambda.Function construct accepts properties like runtime, code and handler. You can explore the various options using your IDE's auto-complete or in the online documentation.

## Useful commands

- `npm run build` compile typescript to js
- `npm run watch` watch for changes and compile
- `npm run test` perform the jest unit tests
- `cdk deploy` deploy this stack to your default AWS account/region
- `cdk diff` compare deployed stack with current state
- `cdk synth` emits the synthesized CloudFormation template
