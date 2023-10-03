# Fargate scheduled task tech test

For this challenge, we would like you to write a CloudFormation template that meets the following requirements:

* Defines a scheduled Fargate task that runs once per minute. The Fargate task must print a Random Useless Fact obtained from this public API: https://uselessfacts.jsph.pl/api/v2/facts/random to stdout. Only the "text" portion of the API response needs to be printed.
* The Fargate task container must be configured to send stdout to CloudWatch Logs. The reviewer of your submission will check CloudWatch Logs for the expected output.
* The CloudFormation stack should provide the CloudWatch Log Group name associated with the previous item in it's Outputs.
* In this repo you will also find [our CloudFormation style guide](cloudformation-style-guide.md), which goes over the basic CloudFormation guidelines we follow as a company. Please review those and ensure the CloudFormation template(s) you are creating follow the guidelines.
* Be well tested!

In addition to the CloudFormation template, we would also like you to fill in the [Submission Description](#submission-description) section of this README with a brief description of what you're submitting. At a minimum, you should include a description of the architecture and how to deploy it, but feel free to include anything you feel is relevant to the reviewer.

> ❗️ If you're unclear about the requirements or expectations in any way, please reach out and let us know. Being inquisitive and detail-oriented will only make you look better in our eyes, so don't be shy!

## Assumptions

Please assume the following conditions when creating the template:

* The VPC/subnet(s) have already been deployed and their IDs can be provided via parameters
* The provided subnet(s) already have access to the internet via a NAT Gateway
* The template **should not** assume the existence of a default VPC.

## Submission Instructions

Please create a zip file containing the CloudFormation template and any other required files and send it to Cloud303.

Please note that the reviewer will attempt to deploy your template, so please ensure that your code is portable across AWS accounts and regions. 

---

## Submission Description

> This section should be filled in by the candidate
