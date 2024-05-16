#prog #info

[[Chaining]] is a [[hash collisions]] resolution technique in [[hash table]]s where each bucket in the [[hash table]] is a [[linked list]]. When a collision occurs (i.e., when two keys [[Hash]] to the same index), the collided elements are stored in the same bucket as a [[linked list]]. Each [[node]] in the [[linked list]] contains a [[key-value pair]].

**Insertion:**
1. [[Hash]] the key to find the appropriate bucket.
2. If the bucket is empty, create a new [[node]] with the [[key-value pair]] and insert it into the bucket.
3. If the bucket is not empty, traverse the [[linked list]]. If the key already exists, update the corresponding value. If not, add a new [[node]] at the end of the [[linked list]].

**Search:**
1. [[Hash]] the key to find the bucket.
2. Traverse the [[linked list]] in the bucket to find the key. If found, return the corresponding value. If not, the key does not exist in the [[hash table]].

**Deletion:**
1. [[Hash]] the key to find the bucket.
2. Traverse the [[linked list]] to find the [[node]] with the corresponding key.
3. If found, remove the [[node]] from the [[linked list]]. If the [[linked list]] becomes empty after deletion, set the bucket to null or a special marker indicating an empty bucket.

**Pros:**
1. Simple Implementation: [[Chaining]] is easy to implement and manage.
2. Low [[Clustering]]: Since elements are stored in [[linked lists]], there is minimal [[Clustering]], even with a high load factor.
3. Efficient for a Broad Range of Operations: [[Chaining]] provides efficient insertion, search, and deletion operations, especially when the number of collisions is low.

**Cons:**
1. Memory Overhead: [[Chaining]] requires additional memory to store pointers/references for [[linked lists]], which can be a concern for large datasets.
2. Cache Inefficiency: Due to scattered memory allocation for [[linked lists]], caching efficiency might be lower compared to [[open addressing]] methods.
3. Inefficiency for Small Datasets: Chaining might not be the most efficient for small datasets, especially when the overhead of [[linked lists]] outweighs the benefits of collision resolution.
