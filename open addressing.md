#prog #info 
Open addressing is a [[Hash collisions|collision]] resolution technique in hash tables where all elements are stored directly in the table itself. When a collision occurs (i.e., when two keys hash to the same index), [[open addressing]] searches for the next open slot in the [[hash table]] to place the collided element. There are several methods for open addressing, including [[linear probing]], [[quadratic probing]], and [[double hashing]].

**Pros:**
1. Simple implementation.
2. Memory-efficient as it uses the same table for storing elements.
3. Cache-friendly due to contiguous memory usage.

**Cons:**
1. [[Clustering]]: [[Open addressing]] can lead to [[Clustering]], where consecutive elements cluster together, increasing the likelihood of further collisions.
2. Efficiency: [[Performance]] may degrade when the table is nearly full, and finding an empty slot becomes challenging.
3. Difficulty in Deletion: Deleting elements requires special handling (like [[tombstones]]) to avoid disrupting the probing sequence.

