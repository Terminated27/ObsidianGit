#prog #info 
**Key-Value Pair: Atomic Note**

A **key-value pair** is a fundamental [[data]] structure in computer science and programming where two pieces of [[data]] are associated with each other. 

- **Key:** The key is a unique identifier or label used to access the associated value. Keys must be distinct within the context of the [[data structure]].
  
- **Value:** The value is the [[data]] or information associated with the key. It can be of any [[data]] type, such as numbers, strings, objects, or even another key-value pair, depending on the specific application.

**Characteristics:**

1. **Uniqueness:** Each key in a collection must be unique. Different keys correspond to different values.

2. **Accessibility:** Values are accessed or retrieved using their corresponding keys. This enables efficient [[data]] retrieval and manipulation.

3. **Flexibility:** Values can be of any [[data]] type or structure, providing flexibility in storing various types of information.

4. **Association:** Key-value pairs establish a direct association between a piece of [[data]] (value) and a way to reference or identify it (key).

**Common Use Cases:**

1. **Databases:** Key-value pairs are used in databases for quick [[data]] retrieval. Keys serve as unique identifiers for database records, allowing rapid access to specific information.

2. **Programming:** In programming, dictionaries, [[Hash]] tables, and associative arrays use key-value pairs to store and manage [[data]] efficiently.

3. **Configuration Settings:** Key-value pairs are often used in configuration files where keys represent settings or parameters, and values contain corresponding values or options.

4. **Caching:** Key-value stores are used in caching mechanisms where frequently accessed [[data]] is stored with a unique key for quick retrieval, improving application [[performance]].

**Example ([[Python]] Object):**

```python
person = {
    "name": "Alice",
    "age": 30,
    "city": "New York"
};
```

In this example, `"name"`, `"age"`, and `"city"` are keys, and `"Alice"`, `30`, and `"New York"` are their respective values. This key-value pairing allows easy access and manipulation of the associated [[data]].