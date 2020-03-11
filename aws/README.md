Provision a Pre-requisite AWS Account
---------------------------------------

This directory launches a pre-requisite AWS stack which includes the RDS database, EFS, EKS cluster, IAM roles, etc. This can be a huge hassle to build by hand individually.

This uses the AWS CDK so it can speak outside and inside EKS.

# Getting Started

## Install AWS CDK

You require the AWS Cloud Development Kit here: https://aws.amazon.com/cdk/

### Launch stack
The `cdk.json` file tells the CDK Toolkit how to execute your app.

First build out all the typescript files into javascript:
```
npm run build
```

Now launch the stack:
```
cdk deploy
```

### Other useful commands

 * `npm run build`   compile typescript to js
 * `npm run watch`   watch for changes and compile
 * `npm run test`    perform the jest unit tests
 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk synth`       emits the synthesized CloudFormation template
