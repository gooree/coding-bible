# Apache Kafka

# Start kafka server
kafka-server-start.sh /etc/kafka/server.properties

# Create a topic
kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic test

# Show topic list
kafka-topics.sh --list --zookeeper localhost:2181

# Send some message
kafka-console-producer.sh --broker-list localhost:9092 --topic test

# Start a consumer
kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning
