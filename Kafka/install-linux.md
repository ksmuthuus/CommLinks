# Linux - Installation

## In summary, for Linux (ex: Ubuntu)

### Download and Setup Java 8 JDK

```sh
sudo apt install openjdk-8-jdk
```

### Download & Extract the Kafka binaries from <https://kafka.apache.org/downloads>

```sh
wget http://apachemirror.wuchna.com/kafka/2.4.1/kafka_2.11-2.4.1.tgz
tar -xzf kafka_2.11-2.4.1.tgz
mv kafka_2.11-2.4.1 kafka
rm kafka_2.11-2.4.1.tgz
```

### Try Kafka commands using

```sh
bin/kafka-topics.sh
```

### Edit PATH to include Kafka (in ~/.bashrc for example)

1. PATH="$PATH:/your/path/to/your/kafka/bin"

```sh
cd ~
ll
nano .bash_profile
```

### Edit Zookeeper & Kafka configs using a text editor

1. zookeeper.properties: dataDir=/your/path/to/data/zookeeper
1. server.properties: log.dirs=/your/path/to/data/kafka

### Start Zookeeper in one terminal window

```sh
zookeeper-server-start.sh config/zookeeper.properties
```

### Start Kafka in another terminal window

```sh
kafka-server-start.sh config/server.properties
```
