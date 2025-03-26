# HashMap
In Java, HashMap is part of the Java Collections Framework and is found in the java.util package. 
It provides the basic implementation of the Map interface in Java. HashMap stores data in (key, value) pairs. Each key is associated with a value, and you can access the value by using the corresponding key.

Internally uses Hashing (similar to Hashtable in Java).
Not synchronized (unlike Hashtable in Java) and hence faster for most of the cases.
Allows to store the null keys as well, but there should be only one null key object, and there can be any number of null values.
Duplicate keys are not allowed in HashMap, if you try to insert the duplicate key, it will replace the existing value of the corresponding key. 
HashMap uses keys in the same way as an Array uses an index.
HashMap allows for efficient key-based retrieval, insertion, and removal with an average O(1) time complexity.

Characteristics of HashMap

A HashMap is a data structure that is used to store and retrieve values based on keys. Some of the key characteristics of a hashmap include:

Not ordered: HashMaps are not ordered, which means that the order in which elements are added to the map is not preserved. However, LinkedHashMap is a variation of HashMap that preserves the insertion order.
Thread-unsafe: HashMaps are not thread-safe, which means that if multiple threads access the same hashmap simultaneously, it can lead to data inconsistencies. If thread safety is required, ConcurrentHashMap can be used.
Capacity and load factor: HashMaps have a capacity, which is the number of elements that it can hold, and a load factor, which is the measure of how full the hashmap can be before it is resized.


Time and Space Complexity
HashMap provides constant time complexity for basic operations, get and put if the hash function is properly written and it disperses the elements properly among the buckets. Iteration over HashMap depends on the capacity of HashMap and the number of key-value pairs. It is directly proportional to the capacity + size. Capacity is the number of buckets in HashMap. So it is not a good idea to keep a high number of buckets in HashMap initially.
