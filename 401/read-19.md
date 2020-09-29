### Message queues
A message queue is a form of asynchronous service-to-service communication used in serverless and microservices architectures. Messages are stored on the queue until they are processed and deleted. Each message is processed only once, by a single consumer. Message queues can be used to decouple heavyweight processing, to buffer or batch work, and to smooth spiky workloads

### Advantages of Message Queue

Message Queues are important because they help in implementing “decoupling”. Two or more applications are decoupled if they can communicate to each other without being connected. Also, one application is unaware of implementation of other application. In other words, there is no dependencies between them.

**With decoupled applications:** <br>
1 - `Any changes made to one application doesn’t affect other application as long as communication contract is not breached` <br/>
2 - `We can break one monolith application into smaller applications which reduces overall complexity. `<br/>
3 - `it becomes easier to maintain and debug applications.` <br/>
4 - `We can have cross platform applications. Smaller applications can be independently developed in any programming languages and scaled.`

## Message Queue Reliability

With message queue, there is increase in reliability and performance of the system. Producers don’t have to wait for consumers to become available and can add requests in the queue. Consumers can process the message when they are available. No overhead in waiting. MQ are persisting the messages so even if different application components go down, no data will be lost and system will be more fault tolerant.
