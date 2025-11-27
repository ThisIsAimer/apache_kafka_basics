# cmds
## get docker random uuid
- docker run --rm apache/kafka:4.1.0 kafka-storage random-uuid  (docker run --rm apache/kafka:4.1.0 /opt/kafka/bin/kafka-storage.sh random-uuid)
(gets uuid)
- docker run -it --rm apache/kafka:4.1.0 bash
- find / -name "kafka-storage.*" 2>/dev/null

## run kafka cluster
- docker run --rm -v "%cd%\kafka_data:/tmp/kraft-data"  apache/kafka:4.1.0 /opt/kafka/bin/kafka-storage.sh format --cluster-id sqynJkB6QPC-tFX8c_15QQ --config opt/kafka/config/server.properties --standalone 
- success message (Formatting dynamic metadata voter directory /tmp/kraft-combined-logs with metadata.version 4.1-IV1.)