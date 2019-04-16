# Twitter Stream Code

#### TweetKafka
###### Following tutorial by Walker Rowe (BMC Blogs)

Start Zookeeper server (CLI)
bin/zookeeper-server-start.sh config/zookeeper.properties

Start Kafka server (CLI)
bin/kafka-server-start.sh config/server.properties

To create Kafka topic (CLI)
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic *topic_name*

Start streaming by running the code

To consume Kafka messages (CLI)
bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic *topic_name* --from-beginning

#### TweetGrab

Start streaming by running the code
