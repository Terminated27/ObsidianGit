#prog #info 
(BFS)

**Definition:**
Breadth-First Search (BFS) is an algorithm used for traversing or searching [[tree]] or [[Graph]] [[data]] structures. It starts at the [[tree]] [[root]] (or an arbitrary [[node]] in the case of a [[Graph]]), explores all the neighbor nodes at the present depth before moving to nodes at the next depth level.

**Algorithm:**
1. Create a [[queue]] [[data structure]] to maintain the nodes to be explored.
2. [[Enqueue]] the starting [[node]] into the [[queue]].
3. Loop until the [[queue]] is empty:
    - [[Dequeue]] a [[node]] from the [[queue]].
    - Process the [[node]] (e.g., print its value).
    - [[Enqueue]] all the adjacent nodes of the dequeued [[node]] that have not been visited yet.
    - Mark the dequeued [[node]] as visited to avoid processing it again.

**Example in [[Python]]:**

```python
from collections import defaultdict, deque

class Graph:
    def __init__(self):
        self.graph = defaultdict(list)
    
    def add_edge(self, u, v):
        self.graph[u].append(v)
    
    def bfs(self, start):
        visited = [False] * (max(self.graph) + 1)
        queue = deque()
        queue.append(start)
        visited[start] = True
        
        while queue:
            node = queue.popleft()
            print(node, end=" ")  # Process the node
            for neighbor in self.graph[node]:
                if not visited[neighbor]:
                    queue.append(neighbor)
                    visited[neighbor] = True

# Example usage
g = Graph()
g.add_edge(0, 1)
g.add_edge(0, 2)
g.add_edge(1, 2)
g.add_edge(2, 0)
g.add_edge(2, 3)
g.add_edge(3, 3)

print("BFS starting from vertex 2:")
g.bfs(2)
```

**Output:**
```
BFS starting from vertex 2:
2 0 3 1 
```

In this example, the BFS algorithm starts from vertex 2 and explores the [[Graph]] in a breadth-first manner, visiting nodes 2, 0, 3, 1 in that [[order]].
