# AWS CloudFormation for IaC

## Introduction
The goal with this project was the creation and automation of common AWS services through CloudFormation and the AWS CLI.

## Technologies 
* AWS CloudFormation 
* Github Repository 
* AWS CLI

## Setup
1. Pull code 
```
$ git clone https://github.com/rjmazurik/AWS 
```
2. Create stack
```
$ aws cloudformation create-stack --stack-name my-ec2-stack --template-body file://.\AWS\CloudFormation\EC2InstanceWithEBSVolume.YAML
```
3. List properties of all running stacks
```
$ aws cloudformation describe-stacks
```
4. Delete stack when complete
```
$ aws cloudformation delete-stack --stack-name my-ec2-stack
