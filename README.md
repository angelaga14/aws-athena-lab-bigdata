# AWS Athena Laboratory – Big Data

## Overview
This laboratory demonstrates how Amazon Athena can be used to query large datasets stored in Amazon S3, create analytical views, and deploy infrastructure using AWS CloudFormation.

## Technologies Used
- Amazon Athena
- AWS CloudFormation
- AWS CLI
- AWS IAM
- Amazon S3

## CloudFormation Template Deployment

### Validate Template
aws cloudformation validate-template --template-body file://athenaquery.cf.yml

### Create Stack
aws cloudformation create-stack --stack-name athenaquery --template-body file://athenaquery.cf.yml

### List Named Queries
aws athena list-named-queries

### Get Named Query Details
aws athena get-named-query --named-query-id <NamedQueryId>

## Cost Model
Amazon Athena charges $5 per TB of data scanned. Queries in this lab scanned approximately 9.32 GB, resulting in a minimal estimated cost.

## Author
Angela Gonzalez
Universidad Autónoma de Guadalajara
