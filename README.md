# Send-Fanout-Event-Notifications-with-SQS-and-SNS

## Introduction
This tutorial demonstrates how to implement a fanout messaging scenario using Amazon Simple Notification Service (SNS) and Amazon Simple Queue Service (SQS). In this scenario, messages are pushed to multiple subscribers, enabling parallel, asynchronous processing and eliminating the need for periodic polling.

In the context of an online store, whenever an order is placed, an SNS topic is triggered, and multiple SQS queues receive identical notifications, allowing different services to process the order details simultaneously.

This tutorial utilizes AWS services within the AWS Free Tier to help you get started at no cost.

---
## Cost to Complete
The services used are part of the AWS Free Tier:

1,000,000 publishes for Amazon SNS
1,000,000 requests for Amazon SQS
Check AWS Free Tier details here.

## Services Used
Amazon SNS (Simple Notification Service)
Amazon SQS (Simple Queue Service)

## Implementation
Follow the steps outlined in this repository to set up and implement fanout event notifications using Amazon SNS and SQS. The tutorial walks you through creating an SNS topic, subscribing SQS queues to that topic, and sending notifications to the queues.

### Steps
1. Create an SNS Topic: Learn how to create an SNS topic that will serve as the publisher for event notifications.
2. Create SQS Queues: Set up multiple SQS queues that will receive the notifications from the SNS topic.
3. Subscribe Queues to SNS Topic: Link the SQS queues to the SNS topic to receive messages automatically.
4. Send Notifications: Test the setup by publishing a message to the SNS topic when an order is placed.
![message received on endpoint](https://github.com/user-attachments/assets/d8e40943-6850-43fa-b0ca-b41d926ae4e8)

---
## Requirements
- An AWS account
- Basic knowledge of AWS services like SNS and SQS
- AWS CLI or Console access
