#prog #info 

- **Definition:** Dijkstra's Algorithm is a popular algorithm in computer science and mathematics used for finding the shortest path between nodes in a [[Graph]], which may represent, for example, road networks. It ensures that the path chosen is the most efficient in terms of the total distance.

- **Objective:** To find the shortest path from a single source [[node]] to all other nodes in a weighted [[Graph]], where the weights represent the distance between nodes.

- **Key Concepts:**
  1. **[[Graph]] Representation:** The problem is represented as a [[Graph]], with nodes representing locations and edges representing the connections between them, each labeled with a numerical weight.
  
  2. **Optimal Substructure:** Dijkstra's Algorithm builds the shortest path [[tree]] one vertex at a time. At every step, it selects the vertex with the smallest distance from the source and adds it to the shortest path [[tree]].
  
  3. **Greedy Approach:** It uses a greedy approach by always selecting the [[node]] with the smallest known distance from the source, which ensures that the shortest path to every [[node]] is found efficiently.
  
- **Steps:**
  1. **Initialization:** Set the distance to the source [[node]] as 0 and all other nodes' distances as infinity.
  
  2. **Relaxation:** For each [[node]], update its distance value to the source [[node]] if a shorter path is found through the current [[node]].
  
  3. **Selection:** Choose the [[node]] with the smallest distance as the next "current" [[node]] and repeat the relaxation step for its neighbors.
  
  4. **Termination:** When all nodes have been visited, the algorithm terminates, and the shortest paths are known.

- **Complexity:**
  - **Time Complexity:** O(V^2) for the basic version, where V is the number of vertices. With min-[[heap]] [[data structure]], it can be reduced to O((V + E) log V), where E is the number of edges.
  
  - **Space Complexity:** O(V), as it requires storage space proportional to the number of vertices for the distances and parent pointers.

- **Applications:**
  - **[[Routing]] and Networking:** Used in routers to find the shortest path for [[data packet]]s.
  
  - **Maps and Navigation:** Employed in GPS systems to find the shortest route between two locations.
  
  - **Traffic Engineering:** Helps optimize traffic flow by finding the quickest routes for vehicles.

- **Advantages:**
  - **Optimality:** Dijkstra's Algorithm guarantees the shortest path from the source to every other [[node]].
  
  - **Versatility:** It can handle graphs with varying edge weights, making it applicable in diverse real-world scenarios.
  
- **Limitations:**
  - **Non-Negative Weights:** It only works with graphs where all edge weights are non-negative. Negative weights can lead to incorrect results.
  
  - **Resource Intensive:** In its basic form, the algorithm becomes inefficient for very large graphs due to its quadratic time complexity.
