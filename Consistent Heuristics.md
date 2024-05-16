
## Definition

heuristics can be defined as consistent, or monotone, if its estimate is always less than or equal to the estimated distance from any neighboring vertex to the goal, plus the cost of reaching that neighbor.

Formally, for every [[node]] N and each successor P of N, the estimated cost of reaching the goal from N is no greater than the step cost of getting to P plus the estimated cost of reaching the goal from P. That is:

$$
\begin{align}
h(N) &\le c(N,P) +h(P)\\
h(G) &=0
\end{align}
$$
where
- h is the consistent [[heuristic function]]
- N is any [[node]] in the [[graph]]
- P is any descendant of N
- G is any goal [[node]]
- c(N,P) is the cost of reaching [[node]] P from N

A consistent [[heuristic]] is also admissible, i.e. it never overestimates the cost of reaching the goal (the converse, however, is not always true). Assuming non negative edges, this can be easily proved by induction.
https://en.wikipedia.org/wiki/Consistent_heuristic
## Examples

One example of consistent heuristics in computing is the A* algorithm, which is commonly used in pathfinding problems. A* uses a [[heuristic function]] to estimate the distance between two points, allowing it to make informed decisions about which path to take. The [[heuristic function]] must be consistent for A* to work correctly; otherwise, it may lead to incorrect or suboptimal solutions.

In number theory, consistent heuristics can be seen in [[algorithms]] used for prime number factorization. For example, the Pollard's p-1 algorithm uses a [[heuristic]] approach by attempting to find factors of a given number by testing if it is divisible by numbers with specific properties. This approach is based on observations and patterns found in prime numbers and has been shown to produce consistent results.



## Key Concepts & Keywords

- [[Heuristic]] [[algorithms]]
- Approximate solutions
- Constraints
- Objectives
- Validity
- Relevance
- A* algorithm
- Pathfinding problems
- [[Heuristic function]]
- Consistency 
- Prime number factorization 
- Pollard's p-1 algorithm 
- Divisibility 
- Patterns 

## Conclusion

Consistent heuristics play a crucial role in computing and number theory, allowing for the efficient and accurate solution of complex problems. By ensuring that the solutions found are always consistent with the problem's constraints and objectives, these [[algorithms]] provide a reliable approach to finding approximate solutions. Understanding the concept of consistent heuristics is essential for any programmer or mathematician working in these fields.