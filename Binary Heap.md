#info #prog #computing 

A binary [[heap]] is a [[data structure]] that is commonly used in computing and number theory classes. It is a type of [[tree]]-based [[data structure]] that is used to efficiently store and retrieve data in a specific order. In this atomic note, we will explore the key concepts and keywords related to binary heaps, as well as provide clear explanations and relevant examples.

## Definition
A binary [[heap]] is a complete binary [[tree]] where the value of each parent [[node]] is either greater than or equal to (max [[heap]]) or less than or equal to (min [[heap]]) the values of its child nodes. This property is known as the **[[heap]] property**.

## Implementation
Binary heaps can be implemented using arrays or [[linked lists]]. In this note, we will focus on the [[array]] implementation as it is more commonly used.

To represent a binary [[heap]] using an [[array]], we first start by storing the [[root]] [[node]] at index 0. Then, for any given [[node]] at index i:
- Its left child will be located at index 2i+1
- Its right child will be located at index 2i+2
- Its parent will be located at index floor((i-1)/2)

## Operations
The two main operations performed on a binary [[heap]] are **insertion** and **deletion**.

### Insertion
To insert a new element into a binary [[heap]], we first add it to the bottommost level of the [[tree]] at the leftmost available position. Then, we compare its value with its parent's value and swap them if necessary to maintain the [[heap]] property. This process is known as **heapify-up**.

```java
// Java implementation of insertion in a max heap
public void insert(int value) {
    // Add new element to bottommost level of tree
    heapArray[size] = value;

    // Heapify-up: compare value with parent's value and swap if necessary
    int current = size;
    while (heapArray[current] > heapArray[parent(current)]) {
        swap(current, parent(current));
        current = parent(current);
    }
    size++;
}
```

### Deletion
To delete an element from a binary [[heap]], we first remove the [[root]] [[node]] and replace it with the last element in the [[heap]]. Then, we compare this new [[root]] [[node]] with its children and swap it with the larger (max [[heap]]) or smaller (min [[heap]]) child to maintain the [[heap]] property. This process is known as **heapify-down**.

```java
// Java implementation of deletion in a max heap
public int delete() {
    // Remove root node and replace with last element in heap
    int deletedValue = heapArray[0];
    heapArray[0] = heapArray[size-1];
    size--;

    // Heapify-down: compare new root node with children and swap if necessary
    int current = 0;
    while (current < size && !isLeaf(current)) {
        int largerChildIdx = getLargerChildIdx(current);
        if (heapArray[current] < heapArray[largerChildIdx]) {
            swap(current, largerChildIdx);
            current = largerChildIdx;
        } else {
            break;
        }
    }
    
    return deletedValue;
}
```

## Example
Let's consider the following binary max [[heap]]:

$$
\begin{matrix}
16 & 14 & 10 & 8 & 7 & 9 & 3 & 2 & 4 & 1 
\end{matrix}
$$

To insert a new element with value 15 into this max [[heap]], we would first add it to the bottommost level at the leftmost available position:

$$
\begin{matrix}
16 & 14 & 10 & 8 & 7 & 9 & 3 & 2 & 4 & 1 & 15
\end{matrix}
$$

Then, we would compare its value (15) with its parent's value (8) and swap them if necessary:

$$
\begin{matrix}
16 & 14 & 10 & \color{red}{15} & 7 & 9 & 3 & 2 & 4 & \color{red}{8} & \color{red}{1}
\end{matrix}
$$

Next, we would compare the new parent's value (15) with its parent's value (14) and swap them if necessary:

$$
\begin{matrix}
16 & \color{red}{15} & \color{red}{10} & \color{red}{14} & \color{red}{7} & 9 & \color{red}{3} &
2 &
4 &
8 &
1
\end{matrix}
$$

Finally, we would compare the new parent's value (16) with its children's values (15 and 10) and swap it with the larger child to maintain the [[heap]] property:

$$
\begin{matrix}
\color{red}{16} &
10 &
14 &
7 &
15 &
9 &
3 &
2 &
4 &
8 &
1
\end{matrix}
$$



