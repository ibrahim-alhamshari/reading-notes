# Amazon SNS

> Amazon Simple Notification Service (Amazon SNS) is a fully managed messaging service for both application-to-application (A2A) and application-to-person (A2P) communication.

- **Benefits**
1. Modernize and decouple your applications
2. Send messages directly to millions of users
3. Reliably deliver messages
4. Automatically scale your workload
5. Ensure accuracy with message ordering and deduplication
6. Simplify your architecture with Message Filtering

-  AWS SNS uses the Publisher-Subscriber model to send messages to its endpoints. Using Amazon SNS, you can filter the messages to a larger number of subscribers or end points through mobile messages, SMS, and email.

- Steps that are Implemented by AWS SNS:
    1) First, the publisher sends out the required notifications that are to be delivered to subscribers.
    2) The published messages are delivered to the SNS service
    3) The subscriber receives the message through subscribing queues or microservices. Subscribers provide useful information such as URL address, email address, or phone number in order to receive the message.

- Steps to implement message filtering with Amazon SNS service:
    1) Create an Amazon SNS Topic.
    2) Create the Amazon SQS Queues
    3) Subscribe the Queues to the Topic
    4) Set Filter Policies to the SNS Subscriptions
    5) Publish Messages to the Topic
    6) Verify Your Message Deliveries

![SNS](https://d2908q01vomqb2.cloudfront.net/632667547e7cd3e0466547863e1207a8c0c0c549/2021/07/13/image4.png)

### Resources
- [SNS with Amplify](https://aws.amazon.com/blogs/messaging-and-targeting/getting-started-with-push-notifications-using-aws-amplify/)
- [SNS: Getting Started](https://aws.amazon.com/sns/getting-started/)