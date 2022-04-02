# IAM CloudFormation Templates

## Background
Templates that are found within this directory (iam) are specific CloudFormation examples for deploying IAM resources.

## Administrator User (admin_user.yaml)
Within this CFT, CloudFormation will create in total, 5 resources. These resources are:

- `AWS::IAM::Group`: An IAM User Group that will be used for adding a new User to. The purpose is to give everyone within the group, Administrator Privileges.
- `AWS::IAM::User`: An IAM User that will be for creating a new user within the AWS Account. The Password and UserName can be replaced