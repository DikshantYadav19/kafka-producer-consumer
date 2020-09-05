# kafka-producer-consumer

Start zookeeper server
```
zookeeper-server-start.bat config\zookeeper.properties
```

Start kafka server
```
kafka-server-start.bat config\server.properties
```

Once both zookeeper and kafka are running, create topic.
```
kafka-topics --zookeeper 127.0.0.1:2181 --topic first_topic --create --partitions 3 --replication-factor 2
```

List all the kafka topics
```
kafka-topics --zookeeper 127.0.0.1:2181 --list
```
