#prog #compnum #info 
Depth-First Search (DFS) is a popular [[Graph]] traversal algorithm that explores as far as possible along each [[Circuit Branch]] before [[backtracking]]. It is often used in advanced programming classes to solve various [[Graph]]-related problems efficiently. In [[Python]], implementing DFS can be straightforward and intuitive. Let's delve into the key concepts, keywords, and example code related to DFS in the context of an advanced programming [[Class]].

Key Concepts:
1. [[Graph]] Traversal: DFS is a technique to visit all the vertices of a [[Graph]] systematically.
2. [[Backtracking]]: When a dead end is reached or all nodes have been visited in a [[Circuit Branch]], the algorithm backtracks to explore other unvisited branches.
3. [[Stack]]-based Approach: DFS uses a [[stack]] [[data structure]] to keep track of visited nodes and their exploration order.
4. Recursive Implementation: DFS can be implemented recursively by calling the function on adjacent unvisited nodes.

Keywords:
1. [[Graph]]: A collection of nodes/vertices connected by edges.
2. Vertex/[[Node]]: Individual elements within a [[Graph]].
3. Edge: Connects vertices and represents relationships between them.
4. Adjacency List/[[Matrix]]: [[Data]] structures representing [[Graph]] connections.
5. Visited [[Array]]/[[Set]]: A [[data]] structure used to track visited nodes during traversal.

Example Code:

# Define a simple [[Graph]] using adjacency list representation
```python
graph = {
    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': ['F'],
    'F': []
}
```
# Recursive implementation of DFS
```python
def dfs_recursive(graph, start_node, visited):
    if start_node not in visited:
        print(start_node, end=" ")
        visited.add(start_node)
        for neighbor in graph[start_node]:
            dfs_recursive(graph, neighbor, visited)
```

# Iterative implementation of DFS using stack
```python
def dfs_iterative(graph, start_node):
    visited = set()
    stack = [start_node]

    while stack:
        current_node = stack.pop()
        if current_node not in visited:
            print(current_node, end=" ")
            visited.add(current_node)
            stack.extend(graph[current_node])
```

# Example usage
```python
print("DFS Recursive:")
dfs_recursive(graph, 'A', set())

print("\nDFS Iterative:")
dfs_iterative(graph, 'A')
```

Output:
DFS Recursive: A B D E F C
DFS Iterative: A C F B E D

In the given example, we have a [[Graph]] represented using an adjacency list. The DFS algorithm is applied to explore the [[Graph]] starting from [[node]] 'A'. Both recursive and iterative implementations are provided.

Key takeaways:
- Depth-First Search (DFS) is a [[Graph]] traversal algorithm used to systematically visit all vertices of a [[Graph]].
- DFS uses [[backtracking]] and can be implemented using [[recursion]] or iteration with a [[stack]].
- In [[Python]], implementing DFS for an advanced programming [[Class]] involves understanding key concepts like [[Graph]] traversal and [[backtracking]].
- Important keywords related to DFS include [[Graph]], vertex/[[node]], edge, adjacency list/[[Matrix]], and visited [[array]]/[[set]].

