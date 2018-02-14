
# AWS CLI

## How to install and configure AWS CLI

## Installation and configuration

- via pip (we are going to omit this part)
- [via Installer](#installer)

[](#installer)

### Install with installer

Just follow the instruction and reboot after finish, due to the installer appends environment variables. Use `aws --version` to check installation success or not.

### configure it

Before we need to go to AWS IAM console to create an IAM user and as could as possible to use IAM user. IAM user also can log into console or access service. The different between IAM user and root account is IAM users are access restricted. IAM controls what they can access and significantly reduces the exposure probability of root account. That makes your account more safety. Even if the IAM user is hacked, the consequences are more controllable. Think about once root account is hacked, the disaster will be unstoppable.

Using `aws configure --profile adminuser` to configure IAM user. The console will ask about access key id and secret key, you can find in `IAM console > Users > (tag) Security Credentials`.

Then use `aws lambda list-function --profile adminuser` to check if you have the right authority to reach lambda function.
