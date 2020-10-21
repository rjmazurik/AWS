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
$ git clone https://github.com/rjmazurik/AWS/blob/master/CloudFormation/EC2InstanceWithEBSVolume.YAML 
```
2. create stack, append your created key pair for ParameterValue
```
$ aws cloudformation create-stack --stack-name my-ec2-stack --template-body file://~\AWS\CloudFormation\EC2InstanceWithEBSVolume.YAML --parameters ParameterKey=KeyName,ParameterValue=YourKeyPairHere
```
3. List properties of all running stacks
```
$ aws cloudformation describe-stacks
```
4. delete stack when done 
```
$ aws cloudformation delete-stack --stack-name my-ec2-stack
