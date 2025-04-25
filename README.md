# container-aws-typescript

A Pulumi TypeScript project that builds and deploys a simple Node.js application as a Docker container to **AWS Fargate**, with an **ECS Cluster**, **ECR Repository**, and an **Application Load Balancer (ALB)**.

---

## What This Project Includes

-  ECS Cluster using Fargate
-  ECR Repository for container image storage
-  ALB to expose the application to the internet
-  Dockerized Node.js app built from `./app`
-  Pulumi for Infrastructure as Code (IaC) using TypeScript

---

## Prerequisites

Make sure you have the following installed and configured:

- [Node.js](https://nodejs.org/)
- [Pulumi CLI](https://www.pulumi.com/docs/get-started/install/)
- AWS credentials configured using `aws configure` or environment variables

---

## Install Dependencies

```
npm install
```

## pulumi config set containerPort 80
```
pulumi config set containerPort 80
pulumi config set cpu 512
pulumi config set memory 128
```
## Deploy to AWS

```
pulumi up
```


