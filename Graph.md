

Graphs are a fundamental [[data structure]] in computer science that represent a collection of nodes (also known as vertices) connected by edges. They are widely used in various applications, including social networks, transportation systems, and computer networks.

In [[Python]] advanced programming, graphs can be implemented using different data structures such as dictionaries, lists, or classes. In this atomic note, we will focus on using classes to represent graphs and explore some advanced techniques for working with them.

## Creating a Graph [[Class]]

To create a graph [[class]] in [[Python]], we first need to define the basic components of a graph: nodes and edges. We can do this by creating two separate classes for each component:

```python
class Node:
    def __init__(self, value):
        self.value = value
        self.neighbors = []

class Edge:
    def __init__(self, start_node, end_node):
        self.start_node = start_node
        self.end_node = end_node
```

Next, we can create our graph class that will hold all the nodes and edges together:

```python
class Graph:
    def __init__(self):
        self.nodes = []
        self.edges = []

    def add_node(self, value):
        new_node = Node(value)
        self.nodes.append(new_node)

    def add_edge(self, start_value, end_value):
        start_node = None
        end_node = None

        # Find the nodes with the given values in the graph
        for node in self.nodes:
            if node.value == start_value:
                start_node = node
            if node.value == end_value:
                end_node = node

        # If either of the nodes is missing, raise an error
        if not start_node or not end_node:
            raise ValueError("Nodes not found in the graph.")

        # Create an edge between the two nodes and add it to the graph
        new_edge = Edge(start_node, end_node)
        self.edges.append(new_edge)

        # Add the end node as a neighbor to the start node
        start_node.neighbors.append(end_node)
```

## Traversing a Graph

One of the key operations in working with graphs is traversing them, which means visiting each [[node]] and edge in the graph. There are two common ways to traverse a graph: [[depth-first search]] (DFS) and [[breadth-first search]] (BFS).

### [[Depth-First Search]] (DFS)

In DFS, we start at a given [[node]] and explore its neighbors first before moving on to its other neighbors. This process continues until all nodes have been visited.

```python
def dfs(self, start_value):
    # Find the starting node in the graph
    start_node = None
    for node in self.nodes:
        if node.value == start_value:
            start_node = node
    
    # If the starting node is not found, raise an error
    if not start_node:
        raise ValueError("Node not found in the graph.")

    # Initialize an empty stack and add the starting node to it
    stack = []
    stack.append(start_node)

    # Initialize an empty set to keep track of visited nodes
    visited = set()

    while stack:
        # Pop a node from the stack and mark it as visited
        current_node = stack.pop()
        visited.add(current_node)

        # Visit all unvisited neighbors of the current node and add them to the stack
        for neighbor in current_node.neighbors:
            if neighbor not in visited:
                stack.append(neighbor)
    
    return visited
```

### [[Breadth-First Search]] (BFS)

In BFS, we explore all neighbors of a given [[node]] before moving on to their respective neighbors. This process continues until all nodes have been visited.

```python
def bfs(self, start_value):
    # Find the starting node in the graph
    start_node = None
    for node in self.nodes:
        if node.value == start_value:
            start_node = node
    
    # If the starting node is not found, raise an error
    if not start_node:
        raise ValueError("Node not found in the graph.")

    # Initialize an empty queue and add the starting node to it
    queue = []
    queue.append(start_node)

    # Initialize an empty set to keep track of visited nodes
    visited = set()

    while queue:
        # Dequeue a node from the queue and mark it as visited
        current_node = queue.pop(0)
        visited.add(current_node)

        # Visit all unvisited neighbors of the current node and add them to the queue
        for neighbor in current_node.neighbors:
            if neighbor not in visited:
                queue.append(neighbor)
    
    return visited
```
