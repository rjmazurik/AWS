# AWS CloudFormation for IaC

## Introduction
The goal with this project was the creation and automation of common AWS services through CloudFormation and the AWS CLI.

## Technologies 
* AWS CloudFormation 
* Github Repository 
* AWS CLI

## Setup
To run this project install and configure the AWS CLI onto your machine. Secondly clone github repository locally. Finally issue the following commands:
```
$ aws cloudformation create-stack --stack-name (insert name) --template-body file://insertlocalfilepathhere
$ aws cloudformation describe-stacks #list properties of all running stacks 
$ aws cloudformation delete-stack --stack-name (insert name) 
