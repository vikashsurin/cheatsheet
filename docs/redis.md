# Redis

## Service Management

* `sudo systemctl start redis`: Start Redis service
* `sudo systemctl stop redis`: Stop Redis service
* `sudo systemctl restart redis`: Restart Redis service
* `sudo systemctl status redis`: Check the status of Redis service
* `sudo systemctl enable redis`: Enable Redis to start on boot
* `sudo systemctl disable redis`: Disable Redis from starting on boot

## Basic Redis CLI Commands

* `redis-cli`: Start the Redis command-line interface
* `redis-cli -h <host> -p <port>`: Connect to a specific Redis instance
* `redis-cli ping`: Check if Redis is running

## Key-Value Operations

* `SET key value`: Set a string value
* `GET key`: Get the value of a key
* `DEL key`: Delete a key
* `EXISTS key`: Check if a key exists
* `KEYS pattern`: Find all keys matching the given pattern
* `EXPIRE key seconds`: Set a key's time to live in seconds
* `TTL key`: Get the time to live for a key

## List Operations

* `LPUSH key value [value ...]`: Insert all the specified values at the head of the list
* `RPUSH key value [value ...]`: Insert all the specified values at the tail of the list
* `LPOP key`: Remove and get the first element in a list
* `RPOP key`: Remove and get the last element in a list
* `LRANGE key start stop`: Get a range of elements from a list

## Set Operations

* `SADD key member [member ...]`: Add one or more members to a set
* `SMEMBERS key`: Get all the members in a set
* `SREM key member [member ...]`: Remove one or more members from a set
* `SISMEMBER key member`: Check if a member exists in a set

## Hash Operations

* `HSET key field value`: Set the string value of a hash field
* `HGET key field`: Get the value of a hash field
* `HDEL key field [field ...]`: Delete one or more hash fields
* `HGETALL key`: Get all the fields and values in a hash

## Sorted Set Operations

* `ZADD key score member [score member ...]`: Add one or more members to a sorted set
* `ZRANGE key start stop [WITHSCORES]`: Return a range of members in a sorted set
* `ZREM key member [member ...]`: Remove one or more members from a sorted set

## Pub/Sub

* `SUBSCRIBE channel [channel ...]`: Listen for messages published to the given channels
* `PUBLISH channel message`: Post a message to a channel
* `UNSUBSCRIBE [channel [channel ...]]`: Stop listening for messages posted to the given channels

## Transaction Commands

* `MULTI`: Mark the start of a transaction block
* `EXEC`: Execute all commands issued after MULTI
* `DISCARD`: Discard all commands issued after MULTI

## Server Commands

* `INFO`: Get information and statistics about the server
* `CONFIG GET parameter`: Get the value of a configuration parameter
* `CONFIG SET parameter value`: Set a configuration parameter to the given value
* `FLUSHDB`: Remove all keys from the current database
* `FLUSHALL`: Remove all keys from all databases

## Persistence Commands

* `SAVE`: Synchronously save the dataset to disk
* `BGSAVE`: Asynchronously save the dataset to disk
* `LASTSAVE`: Get the UNIX time stamp of the last successful save to disk

## Cluster Commands

* `CLUSTER INFO`: Provide information about the cluster
* `CLUSTER NODES`: Get details about cluster nodes

## Debugging

* `MONITOR`: Listen for all requests received by the server in real-time
* `SLOWLOG GET [number]`: Get the slow logs

## Security

* `AUTH password`: Authenticate to the server

Remember to use appropriate authentication and security measures when working with Redis, especially in production environments.
