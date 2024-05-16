#prog #info 

Binary search is an efficient algorithm for finding a specific value in a sorted [[array]]. It works by repeatedly dividing the portion of the [[array]] that could contain the item being searched for and then comparing the middle element to the target value. Here's how you can implement binary search in [[Python]]:

[[Binary Search Tree]]

**Algorithm:**

1. **Initialize:** Set `left` to the index of the first element in the [[array]] and `right` to the index of the last element.
2. **Iterate:** While `left` is less than or equal to `right`, repeat steps 3-6.
3. **Middle Index:** Calculate the middle index: `mid = (left + right) // 2`.
4. **Check Middle Element:** If the middle element is equal to the target, return the index.
5. **Update Indices:** If the target is less than the middle element, set `right = mid - 1`. If the target is greater, set `left = mid + 1`.
6. **Repeat:** Go back to step 2.

**[[Python]] Implementation:**

```python
def binary_search(arr, target):
    left, right = 0, len(arr) - 1

    while left <= right:
        mid = (left + right) // 2

        # Check if target is present at mid
        if arr[mid] == target:
            return mid

        # If target is greater, ignore left half
        elif arr[mid] < target:
            left = mid + 1

        # If target is smaller, ignore right half
        else:
            right = mid - 1

    # Target is not in the array
    return -1

# Example Usage
sorted_array = [2, 4, 7, 10, 13, 18, 23, 29, 35]
target_value = 13

# Perform binary search
result = binary_search(sorted_array, target_value)

if result != -1:
    print(f"Element found at index {result}")
else:
    print("Element not found in the array")
```

In this example, the `binary_search` function takes a sorted [[array]] (`arr`) and a target value (`target`). It returns the index of the target value if found, otherwise, it returns -1 to indicate that the target is not in the [[array]].
