# Mac OS X - Summary

## In summary, for Mac OS X

### Install brew (if needed)

```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### Download and Setup Java 8 JDK

```sh
brew tap caskroom/versions
brew cask install java8
```

1. Download & Extract the Kafka binaries from <https://kafka.apache.org/downloads>

1. Install Kafka commands using brew: brew install kafka

1. Try Kafka commands using kafka-topics (for example)

1. Edit Zookeeper & Kafka configs using a text editor

```sh
zookeeper.properties: dataDir=/your/path/to/data/zookeeper

server.properties: log.dirs=/your/path/to/data/kafka
```

### Start Zookeeper in one terminal window

```sh
zookeeper-server-start config/zookeeper.properties
```

### Start Kafka in another terminal window

```sh
kafka-server-start config/server.properties
```
