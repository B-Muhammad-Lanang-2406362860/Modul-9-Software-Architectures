## Initiating Subscriber

**a. What is amqp?**

AMQP stands for Advanced Message Queuing Protocol that is used for passing event data. It is like the strict rule so publisher and subscriber can talk safely to the message broker. By using this protocol, we make sure message not get lost when the system is busy.

**b. What does it mean? guest:guest@localhost:5672**

This whole text is the address string used by my program to connect to the RabbitMQ server. The first "guest" is the default username, while the second "guest" is the password for it. Then "localhost" mean the broker machine is running in my own local computer. Finally, the "5672" is the port number where the RabbitMQ is waiting for connection.

## Initiating Publisher

**a. How much data your publisher program will send to the message broker in one run?**

My publisher program will send exactly five event messages to the RabbitMQ message broker. Each message contains a unique data representing a new user: Amir, Budi, Cica, Dira, and Emir.

**b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?**

Yes, the url is the same as that on the subscriber program. Using the identical URL makes both the publisher and the subscriber are connecting to the exact same message broker instance. They will establish a synchronized communication channel where the publisher drops off its data and the subscriber knows exactly where to listen. If they used different URLs, the programs would be completely disconnected from one another.

## Running RabbitMQ as Message Broker

![Running RabbitMQ as Message Broker](assets/01_rabbitmq.png)
