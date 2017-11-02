since `https://github.com/quantifind/KafkaOffsetMonitor` has no release for kafka version > 0.9 which offset stored in kafka topic, here is a mirror for you to monitor kafka partition offset in kafka which version > 0.9.

run this command on you shell, or you can see `https://github.com/quantifind/KafkaOffsetMonitor` for more.

```
java -cp KafkaOffsetMonitor-assembly-0.3.0-SNAPSHOT.jar com.quantifind.kafka.offsetapp.OffsetGetterWeb --offsetStorage kafka --zk localhost:2181 --port 8072 --refresh 10.seconds --retain 2.days 1>stdout.log 2>stderr.log &
```

thank you for your attention.
