# IAM CloudFormation Templates

## Background
Templates that are found within this directory (iam) are specific CloudFormation examples for deploying IAM resources.

## Administrator User (admin_user.yaml)
Within this CFT, CloudFormation will create in total, 5 resources. These resources are:

- `AWS::IAM::Group`: An IAM User Group that will be used for adding a new User to. The purpose is to give everyone within the group, Administrator Privileges.
- `AWS::IAM::User`: An IAM User that will be for creating a new user within the AWS Account. The Password and UserName can be replaced with whatever a user wants - just make sure that you reset your password.
- `AWS::IAM::UserToGroupAddition`: An IAM UserToGroupAddition is a way of adding a user to a group within a CloudFormation Template, especially when you are creating a new group and user.
- `AWS::IAM::VirtualMFADevice`: An IAM VirtualMFADevice is a way of enabling MFA authentication for IAM users.

> `AWS::IAM::VirtualMFADevice` has a bug where it will create a new MFA Device, but will not be able to sync the MFA Device to the user.

