
# CloudFront-S3-WAF
<!--BEGIN STABILITY BANNER-->
---

![Stability: Stable](https://img.shields.io/badge/stability-Stable-success.svg?style=for-the-badge)

> **This is a stable example. It should successfully build out of the box**
>
> This examples is built on Construct Libraries marked "Stable" and does not have any infrastructure
prerequisites to build.

---
<!--END STABILITY BANNER-->

This example creates S3 bucket, CloudFront distribution to host S3 static Website, and WAF Web ACL to restrict access to CloudFront distribution based on IP set.

## Build

To build this app, you need to be in this example's root folder. Then run the following:

```bash
npm install -g aws-cdk
dotnet build
```

This will install the necessary CDK, then this example's dependencies, and then build your .Net
Project files and your CloudFormation template.

## Deploy

Run `cdk deploy CloudFrontS3WafStack`. This will deploy / redeploy your Stack to your AWS Account.

After the deployment you will see the CloudFront URL, which represents the url you can then use.

## Synthesize Cloudformation Template

To see the Cloudformation template generated by the CDK, run `cdk synth CloudFrontS3WafStack`, then check
the output file in the"cdk.out" directory.