# Real-Time-Twitter-AWS-Python

Real Time Stream Processing from the Twitter API using AWS Kinesis, Firehose and DynamoDB

This project aims to provide an easy way in python to connect AWS services to twitter API, stream tweets, parse and process them in real-time. The results are stored dynamically in a DynamoDB table. This service can be used for real-time pipelines and machine learning applications, or simply a large-scale data ingestion service.

The AWS Tools used are Kinesis Streams, DynamoDB, Kinesis-Firehose and S3 services. Kinesis Firehose and S3 can be easily connected to Kinesis streams through the AWS GUI (in the Kinesis Firehose panel). Thus you can have a real-time record for complete tweets, which can be used for additional data sourcing.

Since the jupyter notebooks process data continuously, it is recommended to run them on a separate AWS EC2 instance.

To being with, you need to have:
- An AWS Account set up, and AWS CLI installed and configured to your account
- Created an app on twitter developer, and have the below-mentioned credentials
- The boto3, TwitterAPI and tweepy libraries installed for Python
