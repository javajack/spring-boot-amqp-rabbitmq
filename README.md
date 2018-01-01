# spring-boot-amqp-rabbitmq
spring boot with amqp rabbitmq example

# run rabbitmq in docker using this
docker run -d --name rabbitmq -p 5672:5672 -p 15672:15672 gonkulatorlabs/rabbitmq

# else install rabbitmq on your own

# spring-boot-amqp-messaging

This is a simple spring-boot app that shows how to configure easily RabbitMQ with AMQP for producing and consuming messages
in default format (java serialized) and JSON.

In this sample project every message is sent as JSON and then decoded on one queue as a generic `Message` object and in the other 
one as the original specific class.