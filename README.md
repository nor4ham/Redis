# Redis
Redis is an open-source, in-memory data structure store that can be used as a database, cache, and message broker. It provides high-performance storage and retrieval of data by keeping the entire dataset in memory. Redis supports various data structures like strings, hashes, lists, sets, sorted sets, and more.

To use Redis in Python, you'll need to follow these steps:

<b>Step 1:</b> Install the Redis Python library
You can install the Redis library using pip, the Python package manager. Open your terminal or command prompt and run the following command:
```
pip install redis
```
<b>Step 2:</b> Import the Redis library
In your Python script or program, you need to import the Redis library to use its functionalities. Add the following import statement at the top of your Python file:
```
import redis
```
<b> Step 3:</b> Connect to Redis
To connect to a Redis server, create an instance of the Redis class and pass the host and port of the Redis server as arguments. If you're running Redis on your local machine with default settings, you can connect to it using the following code:
```
r = redis.Redis(host='localhost', port=6379)
```
<b> Step 4: :</b> Use Redis commands
Once connected to Redis, you can use various Redis commands to interact with the data. For example, you can use the set command to store a key-value pair in Redis, and the get command to retrieve the value based on the key. Here's an example that demonstrates these operations:
```
# Set a key-value pair
r.set('mykey', 'Hello Redis!')

# Retrieve the value
value = r.get('mykey')
print(value.decode())  # Output: Hello Redis!
```
Remember to handle exceptions and close the Redis connection when you're done using it.
# Resources
https://redis.io/commands
https://www.youtube.com/watch?v=8A_iNFRP0F4&ab_channel=CBTNuggets
https://www.youtube.com/watch?v=jgpVdJB2sKQ&ab_channel=WebDevSimplified
https://www.youtube.com/watch?v=OqCK95AS-YE&ab_channel=TechWorldwithNana
