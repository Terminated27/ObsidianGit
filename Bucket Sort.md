#prog #software 
- Bucket sort is a [[sorting algorithm]] that works by dividing the input data into a fixed number of equally-sized buckets.
- Each element from the input is placed into its respective bucket based on a specific function or rule.
- After all elements are distributed into the buckets, each bucket is sorted, either using another [[sorting algorithm]] or recursively applying bucket sort.
- Finally, the elements from all buckets are concatenated to produce the sorted output.

Bucket sort is particularly effective when the input data is uniformly distributed across a range of values, and the number of buckets is chosen appropriately. It has an average [[big O notation|time complexity]] of O(n+k), where n is the number of elements and k is the number of buckets.