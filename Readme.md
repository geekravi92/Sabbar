## Description

ConCruise And File Service Apps

## Installation

1. Install nodejs from [here](https://nodejs.org/en/)
2. Install Kafka from [here](https://kafka.apache.org/downloads)
3. Install MySQL from homebrew
    ```bash
    $ brew install mysql
    ```

## Running the dependent tools

```bash
# Get into Kafka Folder
$ cd kafka_2.12-2.0.1

# Start Zookeper
$ bin/zookeeper-server-start.sh -daemon config/zookeeper.properties

# Start Kafka Server
$ bin/kafka-server-start.sh -daemon config/server.properties

# Create a topic
$ bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --config retention.ms=604800000 --topic customers

$ bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --config retention.ms=604800000 --topic drivers

# Start mysql with username = root and password = root
```

## Test

**Yet to be written**

## To Be Completed

**Update, Deletion**
**CLI Commands**

## Further Action

**Go To ConCruise Service to initialize the database and Kafka and start the app**

## Stay in touch

- Author - [Arvind Jaiswal](https://www.linkedin.com/in/arvindjaiswal92/)