# Building Your Own ML Application with AWS Lambda and Amazon SageMaker

In this workshop, we will step through the process of deploying and hosting machine learning (ML) models with AWS Lambda and get on-demand inferences. 

Given a demonstrative dataset, we will build and train a simple ML classification model with Amazon SageMaker. Then, we'll host this model in an AWS Lambda function and expose an inference endpoint through Amazon API Gateway. Finally, we'll build a pipeline for automating model deployment to Lambda leveraging AWS CodeBuild, AWS CodeDeploy, and AWS CodePipeline.

## Prerequisites

### AWS Account

In order to complete this workshop you'll need an AWS Account, and an AWS IAM user in that account with at least full permissions to the following AWS services:

- AWS IAM
- Amazon S3
- Amazon SageMaker
- AWS Cloud9
- AWS Lambda
- AWS CodeBuild
- AWS CodePipeline
- AWS CodeDeploy
- Amazon CloudWatch

**Use Your Own Account:** The code and instructions in this workshop assume only one student is using a given AWS account at a time. If you try sharing an account with another student, you'll run into naming conflicts for certain resources. You can work around these by appending a unique suffix to the resources that fail to create due to conflicts, but the instructions do not provide details on the changes required to make this work. Use a personal account or create a new AWS account for this workshop rather than using an organization’s account to ensure you have full access to the necessary services and to ensure you do not leave behind any resources from the workshop.

**Costs:** Some, but NOT all, of the resources you will launch as part of this workshop are eligible for the AWS free tier if your account is less than 12 months old. See the **[AWS Free Tier](https://aws.amazon.com/free/)** page for more details. To avoid charges for endpoints and other resources you might not need after you've finished a workshop, please refer to this **[Cleanup Guide](https://github.com/awslabs/amazon-sagemaker-workshop/blob/master/CleanupGuide)**.


### AWS Region

Amazon SageMaker is available in the following AWS Regions:  N. Virginia, Oregon, Ohio, Ireland, Frankfurt, Seoul, Sydney, Tokyo and AWS GovCloud (US). However, the instructions assume the selected region is **N. Virginia**.

Once you've chosen a region, you should create all of the resources for this workshop there, including a new Amazon S3 bucket and a new SageMaker notebook instance. Make sure you select your region from the dropdown in the upper right corner of the AWS Console before getting started.

![Region selection screenshot](images/region-selection.png)

### Browser

We recommend you use the latest version of Chrome or Firefox to complete this workshop.

### AWS CLI

To complete certain workshop modules, you'll need the AWS Command Line Interface (CLI) and a Bash environment. You'll use the AWS CLI to interface with AWS services. 

However, for these workshop, you are going to use it from AWS Cloud9 to avoid problems that can arise configuring the CLI on your machine and make easier to deploy a Lambda function. AWS Cloud9 is a cloud-based integrated development environment (IDE) that lets you write, run, and debug your code with just a browser. It has the AWS CLI pre-installed so you don’t need to install files or configure your laptop to use the AWS CLI. 

## Let's get started

Execute the following steps:

1. [Training the Spam Filter model with Amazon SageMaker](training/README.md)
2. [Hosting the model in a Lambda Function and executing inferences](hosting/README.md)
3. [Automating deployment](automating/README.md)

Bonus:

[Building Apache MXNet deployment package for AWS Lambda](building/README.md)

## License

The contents of this workshop are licensed under the [Apache 2.0 License](./LICENSE).


## Authors

[Diego Natali](https://www.linkedin.com/in/diego-natali-63182b35/) - Solutions Architect - Amazon Web Services EMEA<br />
[Giuseppe Porcelli](https://it.linkedin.com/in/giuporcelli) - Sr. Solutions Architect - Amazon Web Services EMEA
