> 下载kafka

    wget http://archive.apache.org/dist/kafka/2.7.0/kafka_2.12-2.7.0.tgz

> start-kafka.sh

    nohup bin/zookeeper-server-start.sh config/zookeeper.properties > /dev/null &
    bin/kafka-server-start.sh -daemon  config/server.properties
