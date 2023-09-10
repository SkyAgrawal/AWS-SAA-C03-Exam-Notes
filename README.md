# AWS-SAA-C03-Exam-Notes

Aakash's notes for AWS SAA C03 Exam notes.

## Services

### IAM Service

IAM stands for _Identity and Access Management_ .

It is a __Global__ service.

In IAM, we create users and assign them to groups.

[AWS IAM User Guide](https://docs.aws.amazon.com/IAM/latest/UserGuide/id.html)

#### Users

Users are people within an organization. 
Users can be assigned to groups.
Users can belong to multiple groups.

##### Root User

It is created by default.

#### Groups

A collection of IAM users.

You can't use a group to sign-in.

You can use groups to specify permissions for multiple users at a time.

Groups make permissions easier to manage for large sets of users.

#### Policy

Policies can be assigned to users or groups.

A policy can be defined as a json document.

A policy allows to provide permissions to users or groups. 

AWS IAM best practice : __Least Privilege Principle__ - don't give more permissions than a user needs.

##### Policy Structure

A policy can be represented by a json document.

A policy contains the following sections:

__Version__ : This represents the version of the policy document language. It should be '2012-10-17'. ( Mandatory )

__Id__ : This represents the id of the policy. ( Optional )

__Statements__ : This can be one or more individual statement in a policy. ( Mandatory )