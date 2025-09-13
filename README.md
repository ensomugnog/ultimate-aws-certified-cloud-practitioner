# UACCP - [NEW] Ultimate AWS Certified Cloud Practitioner CLF-C02 2025 (Stephane Maarek)

Full Practice Exam included + explanations | Learn Cloud Computing | Pass the AWS Cloud Practitioner CLF-C02 exam!

**Course**: [https://www.udemy.com/course/aws-certified-cloud-practitioner-new/](https://www.udemy.com/course/aws-certified-cloud-practitioner-new/)

## Course content

01 - Introduction

- 01 - Course Introduction

- 02 - Creating an AWS Account

- 03 - AWS Account Activation Troubleshooting

- 04 - Important Message

- 05 - About your instructor

02 - Code & Slides Download

- 01 - Code & Slides Download

03 - What is Cloud Computing

- 01 - Traditional IT Overview

- 02 - What is Cloud Computing

- 03 - The Different Types of Cloud Computing

- 04 - AWS Cloud Overview

- 05 - Important AWS Console UI Update

- 06 - Tour of the Console & Services in AWS

- 07 - About the UI changes in the course

- 08 - Shared Responsibility Model & AWS Acceptable Policy

- 09.1 - What is Cloud Computing Quiz

04 - IAM - Identity and Access Management

- 01 - IAM Introduction Users, Groups, Policies

- 02 - IAM Users & Groups Hands On

- 03 - IAM Policies

- 04 - IAM Policies Hands On

- 05 - IAM MFA Overview

- 06 - IAM MFA Hands On

- 07 - AWS Access Keys, CLI and SDK

- 08 - AWS CLI Setup on Windows

- 09 - AWS CLI Setup on Mac

- 10 - AWS CLI Setup on Linux

- 11 - AWS CLI Hands On

- 12 - AWS CloudShell

- 13 - IAM Roles for AWS Services

- 14 - IAM Roles Hands On

- 15 - IAM Security Tools

- 16 - IAM Security Tools Hands On

- 17 - IAM Best Practices

- 18 - Shared Responsibility Model for IAM

- 19 - IAM Summary

- 20.2 - Identity and Access Management Quiz

05 - EC2 - Elastic Compute Cloud

## Repository configuration
Each submodule in this repository contains the code examples of the original course.

### Create new submodules
Create a new repository on Github, then execute the following commands to link the new repository as a submodule of the main repository:

```
$ cd uaccp
$ git submodule add -b master git@github.com:ensomugnog/uaccp-submodule uaccp-submodule
```

Using the **-b** argument means we want to follow the master branch of the new repository, and after running this command we’ll have a new directory named `uaccp-submodule/`, this directory will automaticaly checkout the master branch for you to be ready to make changes.

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
$ git checkout master
```