# Topics
### What is CDK
### Why do we need CDK
### What is CloudFormation
### Getting Started
### Creating first app

# What is CDK
* An AWS CDK app is an application written in TypeScript, JavaScript, Python, Java,
  or C# that uses the AWS CDK to define AWS infrastructure
* The output of an AWS CDK program is a AWS CloudFormation template
# What is Cloud Formation
* AWS CloudFormation gives you an easy way to declare, provision and manage lifecycle of AWS resources by treating
  infrastructure as code
* You create a template that describes all the AWS resources that you want (like Amazon EC2 instances
  or Amazon RDS DB instances), and AWS CloudFormation takes care of provisioning and configuring those
  resources for you.
* You don't need to individually create and configure AWS resources and figure out what's dependent on what;
  AWS CloudFormation handles all of that.
  https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/GettingStarted.Walkthrough.html

## Stacks
* A stack is a collection of AWS resources that you can manage as a single unit. In other words, you can create, update,
  or delete a collection of resources by creating, updating, or deleting stacks.
* Because AWS CloudFormation treats the stack resources as a single unit, they must all be created or deleted successfully for the stack to be created or deleted

# CDK in Details
* An app defines one or more stacks. Stacks (equivalent to AWS CloudFormation stacks)
  contain constructs, each of which defines one or more concrete AWS resources,
  such as Amazon S3 buckets, Lambda functions, Amazon DynamoDB tables, and so on
* The AWS CDK includes the AWS CDK Toolkit (also called the CLI), a command-line tool for working with your AWS
  CDK apps and stacks.
* The AWS CDK includes the AWS CDK Toolkit (also called the CLI)
* The Toolkit provides the ability to convert one or more AWS CDK stacks to AWS CloudFormation templates

# Getting Started

## Prerequisites
### 1) Install AWS cli
https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html
### 2) Provide your credentials and an AWS Region to use AWS CDK
`aws configure`

or

In ~/.aws/config
```
[default]
region=us-west-2
```
In ~/.aws/credentials
```
[default]
aws_access_key_id=AKIAI44QH8DHBEXAMPLE
aws_secret_access_key=je7MtGbClwBF/2Zp9Utk/h3yCo8nvbEXAMPLEKEY
```
### 3) Install the AWS CDK
```
npm install -g aws-cdk
```
```
cdk --version
```

# Create CDK APP
```
cdk init app --language typescript
```
