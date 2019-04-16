# Twitter Stream Code

#### TweetKafka
###### Following tutorial by Walker Rowe (BMC Blogs)

Start Zookeeper server
bin/zookeeper-server-start.sh config/zookeeper.properties

Start Kafka server
bin/kafka-server-start.sh config/server.properties

To create Kafka topic
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic *topic_name*

To consume Kafka messages
bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic *topic_name* --from-beginning
