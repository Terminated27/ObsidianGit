---
aliases:
  - A*
---

A-star, also known as A* search algorithm, is a popular and efficient pathfinding algorithm used in computer science and mathematics. It is commonly used to find the shortest path between two points on a [[graph]] or grid.

## Explanation

A-star is an informed search algorithm, meaning it uses [[heuristic]] information to guide its search towards the goal [[node]]. It combines the advantages of both [[Dijkstra's algorithm]] and Greedy Best-First Search, making it more efficient in finding the shortest path.

The algorithm works by maintaining two lists: an open list and a closed list. The open list contains all the nodes that are yet to be explored, while the closed list contains the nodes that have already been visited. At each step, the algorithm selects the [[node]] with the lowest cost from the open list and expands it by considering its neighboring nodes.

## Example

Let's say we have a grid with obstacles and we want to find the shortest path from point A to point B. We can represent this grid as a [[graph]], where each [[node]] represents a cell on the grid. The edges between nodes represent possible movements (up, down, left, right) from one cell to another.

![[Astar_progress_animation.gif]]

Using A-star, we start at point A and expand its neighboring nodes based on their estimated cost using a [[heuristic function]]. This function takes into account both the actual distance from each [[node]] to point B (known as g-value) and an estimated distance (known as h-value) based on a chosen [[heuristic]] (e.g. Euclidean distance).
![[AstarExampleEn.gif]]
The algorithm then selects a [[node]] as it has the lowest cost among all expanded nodes. We continue this process until we reach point B or there are no more nodes left in the open list.

## Pseudocode

```Java
function reconstruct_path(cameFrom, current)
    total_path := {current}
    while current in cameFrom.Keys:
        current := cameFrom[current]
        total_path.prepend(current)
    return total_path

// A* finds a path from start to goal.
// h is the heuristic function. h(n) estimates the cost to reach goal from node n.
function A_Star(start, goal, h)
    // The set of discovered nodes that may need to be (re-)expanded.
    // Initially, only the start node is known.
    // This is usually implemented as a min-heap or priority queue rather than a hash-set.
    openSet := {start}

    // For node n, cameFrom[n] is the node immediately preceding it on the cheapest path from the start
    // to n currently known.
    cameFrom := an empty map

    // For node n, gScore[n] is the cost of the cheapest path from start to n currently known.
    gScore := map with default value of Infinity
    gScore[start] := 0

    // For node n, fScore[n] := gScore[n] + h(n). fScore[n] represents our current best guess as to
    // how cheap a path could be from start to finish if it goes through n.
    fScore := map with default value of Infinity
    fScore[start] := h(start)

    while openSet is not empty
        // This operation can occur in O(Log(N)) time if openSet is a min-heap or a priority queue
        current := the node in openSet having the lowest fScore[] value
        if current = goal
            return reconstruct_path(cameFrom, current)

        openSet.Remove(current)
        for each neighbor of current
            // d(current,neighbor) is the weight of the edge from current to neighbor
            // tentative_gScore is the distance from start to the neighbor through current
            tentative_gScore := gScore[current] + d(current, neighbor)
            if tentative_gScore < gScore[neighbor]
                // This path to neighbor is better than any previous one. Record it!
                cameFrom[neighbor] := current
                gScore[neighbor] := tentative_gScore
                fScore[neighbor] := tentative_gScore + h(neighbor)
                if neighbor not in openSet
                    openSet.add(neighbor)

    // Open set is empty but goal was never reached
    return failure
```

 In this pseudocode, if a [[node]] is reached by one path, removed from openSet, and subsequently reached by a cheaper path, it will be added to openSet again. This is essential to guarantee that the path returned is optimal if the [[heuristic function]] is admissible but not consistent. If the [[heuristic]] is consistent, when a [[node]] is removed from openSet the path to it is guaranteed to be optimal so the test `tentative_gScore < gScore[neighbor]` will always fail if the [[node]] is reached again.

## Key Concepts & Keywords

- Pathfinding algorithm
- Informed search
- [[Heuristic function]]
- Open list & closed list
- [[Dijkstra's algorithm]]
- Greedy Best-First Search
- g-value & h-value
- Euclidean distance

## Conclusion

In summary, A-star is a powerful algorithm that combines the efficiency of [[Dijkstra's algorithm]] and the informed search of Greedy Best-First Search. It has various applications in computing and number contexts, such as finding the shortest path in maps, games, and robotics. With its use of [[heuristic]] information, A-star can provide faster results compared to other [[algorithms]].