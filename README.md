# UACCP - [NEW] Ultimate AWS Certified Cloud Practitioner CLF-C02 2025 (Stephane Maarek)

Full Practice Exam included + explanations | Learn Cloud Computing | Pass the AWS Cloud Practitioner CLF-C02 exam!

**Course**: [https://www.udemy.com/course/aws-certified-cloud-practitioner-new/](https://www.udemy.com/course/aws-certified-cloud-practitioner-new/)

## Course content

- [x] 01 - Introduction

  - [x] 01 - Course Introduction

  - [x] 02 - Creating an AWS Account

  - [x] 03 - AWS Account Activation Troubleshooting

  - [x] 04 - Important Message

  - [x] 05 - About your instructor

- [x] 02 - Code & Slides Download

  - [x] 01 - Code & Slides Download

- [x] 03 - What is Cloud Computing

  - [x] 01 - Traditional IT Overview

  - [x] 02 - What is Cloud Computing

  - [x] 03 - The Different Types of Cloud Computing

  - [x] 04 - AWS Cloud Overview

  - [x] 05 - Important AWS Console UI Update

  - [x] 06 - Tour of the Console & Services in AWS

  - [x] 07 - About the UI changes in the course

  - [x] 08 - Shared Responsibility Model & AWS Acceptable Policy

  - [x] 09.1 - What is Cloud Computing Quiz

- [x] 04 - IAM - Identity and Access Management

  - [x] 01 - IAM Introduction Users, Groups, Policies

  - [x] 02 - IAM Users & Groups Hands On

  - [x] 03 - IAM Policies

  - [x] 04 - IAM Policies Hands On

  - [x] 05 - IAM MFA Overview

  - [x] 06 - IAM MFA Hands On

  - [x] 07 - AWS Access Keys, CLI and SDK

  - [x] 08 - AWS CLI Setup on Windows

  - [x] 09 - AWS CLI Setup on Mac

  - [x] 10 - AWS CLI Setup on Linux

  - [x] 11 - AWS CLI Hands On

  - [x] 12 - AWS CloudShell

  - [x] 13 - IAM Roles for AWS Services

  - [x] 14 - IAM Roles Hands On

  - [x] 15 - IAM Security Tools

  - [x] 16 - IAM Security Tools Hands On

  - [x] 17 - IAM Best Practices

  - [x] 18 - Shared Responsibility Model for IAM

  - [x] 19 - IAM Summary

- [x] 20.2 - Identity and Access Management Quiz

- [x] 05 - EC2 - Elastic Compute Cloud

  - [x] 01 - AWS Budget Setup

  - [x] 02 - EC2 Basics

  - [x] 03 - Create an EC2 Instance with EC2 User Data to have a Website Hands On [ [uaccp-create-an-ec2-instance-with-ec2-user-data-to-have-a-website-hands-on](https://github.com/ensomugnog/uaccp-create-an-ec2-instance-with-ec2-user-data-to-have-a-website-hands-on) -> [5f79f2ee927ef5b732adec4f467aeb8a3c93f1b1](https://github.com/ensomugnog/uaccp-create-an-ec2-instance-with-ec2-user-data-to-have-a-website-hands-on/commit/5f79f2ee927ef5b732adec4f467aeb8a3c93f1b1) ]
  
  - [x] 04 - EC2 Instance Types Basics

## Repository configuration
Each submodule in this repository contains the code examples of the original course.

### Create new submodules
Create a new repository on Github, then execute the following commands to link the new repository as a submodule of the main repository:

```
$ cd ultimate-aws-certified-cloud-practitioner
$ git submodule add -b main git@github.com:ensomugnog/uaccp-create-an-ec2-instance-with-ec2-user-data-to-have-a-website-hands-on
```

Using the **-b** argument means we want to follow the main branch of the new repository, and after running this command we’ll have a new directory named `uaccp-submodule/`, this directory will automaticaly checkout the main branch for you to be ready to make changes.

### Update main repository with latest submodule changes
First make sure the submodule changes have been commited and pushed to the orign repository, then run the following commands:

```
$ git status
$ git stage .
$ git commit -m 'uaccp-submodule'
$ git push
```

### Clone Repository with submodules
If you want to clone a repository including its submodules you can use the --recursive parameter, use the --jobs parameter to fetch multiple submodules at the same time, download up to 8 submodules at once use --jobs 8

```
$ git clone --recursive --jobs 8 git@github.com:ensomugnog/ultimate-aws-certified-cloud-practitioner.git
```

### Delete a submodule from a repository
Currently Git provides no standard interface to delete a submodule. To remove a submodule `uaccp-submodule` you need to:

```
$ git submodule deinit -f uaccp-submodule
$ rm -rf .git/modules/uaccp-submodule
$ git rm -f uaccp-submodule
```

### Checkout a commit
To checkout a Git commit, you will need the commit hash.

```
$ git checkout 4aa03973d004286558465a8d86bcccfdc7b46505
$ git reset --hard
$ git checkout main
```