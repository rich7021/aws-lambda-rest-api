
# AWS CLI

## How to install and configure AWS CLI

## Installation and configuration

- via pip (we are going to omit this part)
- [via Installer](#installer)

[](#installer)

### Install with installer

Just follow the instruction and reboot after finish, due to the installer appends environment variables. Use `aws --version` to check installation success or not.

### configure it

Before we need to go to AWS IAM console to create an IAM user and as could as possible to use IAM user.

[reason for using IAM](/00.AWS-IAM/README.md)

Using `aws configure --profile adminuser` to configure IAM user. The console will ask about access key id and secret key, you can find in `IAM console > Users > (tag) Security Credentials`.

Then use `aws lambda list-function --profile adminuser` to check if you have the right authority to reach lambda function.
