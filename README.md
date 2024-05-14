# cctv_lambda

Overview
This documentation guides you through the process of setting up an AWS Lambda function that checks for the presence of CCTV footage files in an S3 bucket at specific hours. If the expected files are not found, it sends an SNS notification.

Prerequisites

1. An AWS account with appropriate permissions to create Lambda functions, S3 buckets, and SNS topics.

2. Basic understanding of Python programming.

3. Basic familiarity with AWS Lambda, S3, and SNS services.

Architecture

The architecture consists of an AWS Lambda function triggered periodically using CloudWatch Events. The Lambda function checks for the existence of CCTV footage files in the S3 bucket and sends an SNS notification if files are missing.

Steps

1. Create an S3 Bucket: If you haven't already, create an S3 bucket to store your CCTV footage files.

2. Create an SNS Topic: Create an SNS topic that will be used to send notifications.

3. Write the Lambda Function: Write a Lambda function in Python to check for the existence of CCTV footage files in the S3 bucket and send SNS notifications if files are missing.

4. Configure CloudWatch Events Rule: Set up a CloudWatch Events rule to trigger the Lambda function periodically.

