# AWS SQS vs SNS
### 1-What is the difference betweeen SQS and SNS?
Amazon SQS (Simple Queue Service) is a message queuing service that enables decoupling of components by storing and managing messages in queues. It follows the point-to-point communication model. Amazon SNS (Simple Notification Service) is a pub/sub (publish/subscribe) service that sends messages to multiple subscribers (endpoints) simultaneously, allowing broadcast-type communication. In summary, SQS is for point-to-point messaging, while SNS is for pub/sub messaging.
### 2- What are some use cases for both SNS and SQS?
- SNS supports several end points such as email, sms, http end point and SQS. If you want unknown number and type of subscribers to receive messages, you need SNS.
- SQS queue system, allowing decoupling of components and systems , and can be used as a task queue to manage asynchronous background tasks in applications .
***
# AWS SNS and SQS
### 1-Describe how to use SQS and SNS in a “fanout” pattern.
A "fanout" pattern involves broadcasting a message from a single source to multiple destinations. In AWS, you can achieve this using SNS and SQS together.
### 2-Explain how “push notifications” work, using SNS.
The push system means that you have an event to distribute, for whoever interested of that event news, must subscribe to the event distributer so once a new event occur, a message will be pushed(sent) to all subscribers notifying them of that new event occurring.
***
# SQS and SNS Basics
### How might a large scale, distributed application make use of a Queue system like SQS?
- Asynchronous Processing: The application can offload time-consuming tasks to the queue, allowing it to handle requests quickly and efficiently without waiting for immediate processing.
- Scalability and Load Balancing: Multiple instances of application components can read from the queue, ensuring an even distribution of workload and enabling the application to scale easily with increased demand.
- Fault Tolerance and Reliability: If a component fails, messages in the queue remain safe, and processing can resume once the component is restored, ensuring data integrity and system resilience.

 


