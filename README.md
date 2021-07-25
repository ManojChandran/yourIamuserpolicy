# AWS CLOUDFORMATION YAML
Create a cloudformation template for IAM 

## Set AWS account

Install AWS cli

```
$ sudo apt install awscli
$ aws --version
```
The set your credentials in the following environment variables:

AWS_ACCESS_KEY_ID / AWS_SECRET_ACCESS_KEY /AWS_SESSION_TOKEN (optional)

The following examples show how you configure the environment variables.

Linux, OS X, or Unix

```
$ export AWS_ACCESS_KEY_ID=YOUR_AKID
$ export AWS_SECRET_ACCESS_KEY=YOUR_SECRET_KEY
$ export AWS_SESSION_TOKEN=TOKEN
$ export AWS_REGION=us-east-1
```

Windows

```
C:\> set AWS_ACCESS_KEY_ID=YOUR_AKID
C:\> set AWS_SECRET_ACCESS_KEY=YOUR_SECRET_KEY
C:\> set AWS_SESSION_TOKEN=TOKEN
C:\> set AWS_REGION=us-east-1
```

## CLONE 

clone the repo, using git command.
```
$ git clone https://github.com/ManojChandran/yourIamuserpolicy.git
```
## RUN Template

Create stack using below command

```
$ aws cloudformation create-stack --stack-name prod --template-body file://main.yml --capabilities CAPABILITY_NAMED_IAM
$ aws cloudformation delete-stack --stack-name prod
```