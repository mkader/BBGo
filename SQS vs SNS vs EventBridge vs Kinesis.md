1. AWS SQS: It is a fully managed message queuing service that helps decouple communication between distributed components.

1. AWS SNS: A fully managed publish/subscribe messaging service using topics to send messages to multiple subscribers or endpoints (such as email, Lambda, SQS, and so on).

1. AWS EventBridge: It is a serverless event bus that facilitates the routing of events between AWS services, and applications based on specific routing rules and filters.

1. AWS Kinesis Data Streams: A real-time data streaming service that captures, processes, and analyzes data in near real-time.

How can you choose which service to use?

Here are some basic tips and examples:

1. For massive amounts of events like a clickstream from an application use Kinesis Data Stream

1. For events processed by a single consumer like an image processing job, SQS is a better choice.

1. For sending messages and notifications, SNS is a great choice.

1. For system events such as a new user registration that multiple services must receive and react to, use EventBridge.

<img src="https://substack-post-media.s3.amazonaws.com/public/images/3ecf2600-10d8-4180-8328-8d790fbba0cc_1280x1557.gif">
