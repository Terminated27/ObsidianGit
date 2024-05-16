#prog 
# Introduction
In [[Python]], a heap is a specialized [[tree]]-based [[data structure]] that satisfies the heap property. It is commonly used to efficiently manage and retrieve the minimum or maximum element from a collection of elements. In this atomic note, we will explore the concept of a heap in the context of an advanced programming class.

# Key Concepts

### Heap Property
A heap is based on the concept of a complete [[binary tree]], where all levels are completely filled except possibly for the last level, which is filled from left to right. The heap property states that for every [[node]] `i`, the value at `i` is either greater than or equal to (in a max-heap) or less than or equal to (in a min-heap) the values at its children.

Here is a diagram representing a max-heap:
![[Pasted image 20231109105142.png]]

### Min-Heap and Max-Heap
A min-heap is a heap where each parent [[node]] has a value less than or equal to its children. Conversely, in a max-heap, each parent [[node]] has a value greater than or equal to its children.

### Heap Operations
The main operations performed on heaps include:

1. **Insertion**: Adding an element to the heap while maintaining the heap property.
2. **Deletion**: Removing and returning the minimum (in case of min-heap) or maximum (in case of max-heap) element from the heap while maintaining the heap property.
3. **Heapify**: Reorganizing an [[array]] into a valid heap structure.
4. **[[Heap Sort]]**: Sorting an [[array]] using heaps.

### [[Priority Queue]]
A [[priority queue]] is an abstract [[data]] type that provides efficient access to the minimum (or maximum) element in constant time. Heaps are often used as underlying data structures for implementing priority queues due to their efficient insertion and deletion operations.

# Example: Creating and Manipulating Heaps in [[Python]]

To work with heaps in [[Python]], we can utilize the `heapq` module, which provides functions for creating and manipulating heaps.

### Creating a Min-Heap
To create a min-heap, we can use the `heapify` function from the `heapq` module. Here's an example:

```python
import heapq

# Create a list of elements
elements = [5, 3, 8, 1, 2]

# Convert the list into a min-heap
heapq.heapify(elements)

print(elements)  # Output: [1, 2, 8, 5, 3]
```

### Insertion and Deletion in a Heap
We can insert elements into a heap using the `heappush` function and remove the minimum element using the `heappop` function. Here's an example:

```python
import heapq

# Create an empty heap
heap = []

# Insert elements into the heap
heapq.heappush(heap, 5)
heapq.heappush(heap, 3)
heapq.heappush(heap, 8)
heapq.heappush(heap, 1)

print(heap)    # Output: [1, 3, 8, 5]

# Remove and return the minimum element from the heap
min_element = heapq.heappop(heap)

print(min_element)   # Output: 1
print(heap)          # Output: [3, 5, 8]
```

### [[Heap Sort]]
[[Heap sort]] is an efficient [[sorting algorithm]] that uses heaps to sort an [[array]] in ascending or descending [[order]]. Here's an example of using [[heap sort]] to sort an [[array]]:

```python
import heapq

def heap_sort(array):
    # Convert array into a max-heap (for descending order)
    heapq.heapify(array)

    sorted_array = []
    
    while array:
        sorted_array.append(heapq.heappop(array))
    
    return sorted_array

# Example usage
arr = [5, 3, 8, 1, 2]
sorted_arr = heap_sort(arr)

print(sorted_arr)   # Output: [1, 2, 3, 5, 8]
```

# Conclusion
Understanding the concept of a heap is crucial in advanced programming classes. It provides an efficient way to manage and retrieve the minimum or maximum element from a collection. By utilizing the `heapq` module in [[Python]], we can easily create and manipulate heaps. Additionally, heaps are widely used as underlying [[data]] structures for implementing priority queues and sorting [[algorithms]] like [[heap sort]].