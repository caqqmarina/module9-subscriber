# Subscriber Readme

## What is AMQP?

AMQP (Advanced Message Queuing Protocol) is an open standard application layer protocol for message-oriented middleware. It enables applications to communicate asynchronously by sending messages between them regardless of differences in their platforms, languages, or locations.

AMQP provides:
- Message orientation: treats messages as self-contained units of information
- Queuing: stores messages until the receiving application is ready to process them
- Routing: determines how messages should be delivered to their intended recipients
- Reliability: ensures messages are delivered even during network or application failures
- Security: provides authentication and encryption mechanisms

Common AMQP implementations include RabbitMQ, ActiveMQ, and Azure Service Bus.

## What does `guest:guest@localhost:5672` mean?

This string is a connection URI for an AMQP message broker with the following components:

- **First `guest`**: Username for authentication to the message broker
- **Second `guest`**: Password for authentication to the message broker
- **`localhost`**: The hostname where the message broker (e.g., RabbitMQ) is running, in this case on the same machine
- **`5672`**: The default port number that AMQP servers typically listen on

In RabbitMQ (a popular AMQP implementation), "guest/guest" are the default credentials that come preconfigured, but they're restricted to only work for connections from localhost by default for security reasons.

The complete format is: `amqp://username:password@hostname:port`

![image](https://github.com/user-attachments/assets/da816b92-6349-4c36-b0a8-3bf5eb1365eb)
