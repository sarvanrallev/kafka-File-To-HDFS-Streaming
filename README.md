# kafka-File-To-HDFS-Streaming
Load data from text File to HDFS through Kafka

To load data from local linux system to HDP cluster using kafka can be done by two property files which contain
the information regarding the source file and kafka topic information to produce. 
similarly another one file which contains the details regarding the HDFS url and other information.

To start this streaming as a standalone service we need to start below script in your kafka bin path,
  
  /opt/confluent_5_3_0/bin/connect-standalone /opt/confluent_5_3_0/bin/etc/schema-registry/connect-avro-standalone.properties /opt/confluent_5_3_0/bin/etc/kafka/connect-file-source.properties /opt/confluent_5_3_0/bin/etc/kafka-connect-hdfs/quickstart-hdfs.properties
  
  
