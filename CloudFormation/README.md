# AWS CloudFormation for IaC

## Introduction
The goal with this project was the creation and automation of common AWS services through CloudFormation and the AWS CLI.

## Technologies 
* AWS CloudFormation 
* Github Repository 
* AWS CLI

## Setup
0. configure aws account through CMD, specify default region name to us-west-2
```
aws configure
```

1. Pull code, cd to AWS directory 
```
$ git clone https://github.com/rjmazurik/AWS
$ cd AWS
```
2. Create stack
```
$ aws cloudformation create-stack --stack-name my-ec2-stack --template-body file://CloudFormation/EC2InstanceWithEBSVolume.YAML
```
3. List properties of all running stacks
```
$ aws cloudformation describe-stacks
```
4. Delete stack when complete
```
$ aws cloudformation delete-stack --stack-name my-ec2-stack
```
## Debugging 
1. Access AWS IAM account https://aws.amazon.com/ 
2. All services -> CloudFormation -> my-ec2-stack -> Events -> Status reason 
