cd /usr/hdp/2.5.0.0-1245/kafka/bin

craeting kafka_topic: ./kafka-topics.sh --zookeeper localhost:2181 --create --topic  test_Topic2 --partitions 2 --replication-factor 2

seeing list of kafka topics: ./kafka-topics.sh --list --zookeeper localhost:2181

kafka producer:  ./kafka-console-producer.sh --broker-list localhost:6667 --topic testTopic2

kafka consumer:  ./kafka-console-consumer.sh --zookeeper node1.shinigami.com:2181 -topic testTopic2

