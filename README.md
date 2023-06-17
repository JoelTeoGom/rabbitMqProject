# rabbitMqProject
In this project, we have developed a distributed sensor system using RabbitMQ as the messaging system to manage communication between various components. RabbitMQ is a highly reliable and scalable messaging middleware based on the Advanced Message Queuing Protocol (AMQP). We employ RabbitMQ to facilitate data transfer between distributed sensors and the servers responsible for processing them.

One of the key advantages of utilizing RabbitMQ in our system is its ability to balance the workload across servers. By implementing queues in RabbitMQ, we ensure that messages sent by sensors are evenly distributed among different processing servers. This optimizes system performance by preventing individual server overload and making efficient use of available resources.

Additionally, we have created a specific proxy that employs a tumbling window based on data retrieved from Redis, which we previously stored. Redis is a high-performance in-memory database that we utilize to store and retrieve historical data relevant to our distributed sensor system. This tumbling window mechanism enables us to process data efficiently and timely, maintaining a relevant and up-to-date context for real-time decision-making.

In summary, by combining RabbitMQ for distributed communication and workload balancing, along with a proxy utilizing a Redis-based tumbling window, we have established a highly efficient and reliable system to manage a distributed array of sensors. This approach allows us to process real-time data, optimizing system performance, and making informed decisions based on relevant historical data.
