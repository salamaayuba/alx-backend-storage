Redis
Getting Started
redis-py requires a running Redis server, and Python 3.7+. See the Redis quickstart for Redis installation instructions.

redis-py can be installed using pip via pip install redis.

Quickly connecting to redis
There are two quick ways to connect to Redis.

Assuming you run Redis on localhost:6379 (the default)

import redis
r = redis.Redis()
r.ping()
Running redis on foo.bar.com, port 12345

import redis
r = redis.Redis(host='foo.bar.com', port=12345)
r.ping()
Another example with foo.bar.com, port 12345

import redis
r = redis.from_url('redis://foo.bar.com:12345')
r.ping()
