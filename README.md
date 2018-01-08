# NOTE - THIS IS DEPRECATED - PLEASE USE CircleCI 2.0 for new projects

This repo is out of date. Please see this blog post for how to deploy to ECS from ECR on CircleCI 2.0: https://circleci.com/blog/aws-ecr-auth-support/

---

## Deploy to AWS ECS from ECR via CircleCI 1.0 (Example Project) - Deprecated

This is a "Hello World" Go webapp that provides an example of how to build and test a Dockerized 
web application on [CircleCI](https://circleci.com), push to an AWS EC2 Container Registry, and then deploy to an AWS 
EC2 Container Service cluster.

## Prerequisites

This example utilizes AWS information that you wouldn't really want public. You'll need to 
configure a few CircleCI environment variables before the deploy script will work:

```
AWS_ACCOUNT_ID
AWS_ACCESS_KEY_ID
AWS_SECRET_ACCESS_KEY
```

Additionally, an EC2 Container Service cluster and EC2 Container Registry must already be set up 
on AWS. See the [EC2 Container Service Resources](https://aws.amazon.com/ecs/) and 
[ECS Container Registry Resources](https://aws.amazon.com/ecr/) to get started. You will also need to update the cluster and 
task family names in deploy.sh to match your cluster.
