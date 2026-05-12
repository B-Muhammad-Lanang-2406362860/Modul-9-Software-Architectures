

**a. What is amqp?**
AMQP stands for Advanced Message Queuing Protocol that is used for passing event data. It is like the strict rule so publisher and subscriber can talk safely to the message broker. By using this protocol, we make sure message not get lost when the system is busy.

**b. What does it mean? guest:guest@localhost:5672**
This whole text is the address string used by my program to connect to the RabbitMQ server. The first "guest" is the default username, while the second "guest" is the password for it. Then "localhost" mean the broker machine is running in my own local computer. Finally, the "5672" is the port number where the RabbitMQ is waiting for connection.