---
aliases: [BFS, Breadth First Search]
---
### Breadth First Search
---
- In [[Breadth First Search|BFS]], we start at a vertex $v$ and mark it as having been reached(visited). The vertex $v$ is at this time said to be unexplored.
- A vertex is said to have been explored by an algorithm when the algorithm has visited all vertices adjacent from it. All unvisited vertices adjacent from $v$ are visited next.
- These are new unexplored vertices. Vertex $v$ has now been explored. The newly visited vertices haven't been explored and are put onto the end of a list of unexplored vertices.
- The first vertex on this list is the next to be explored. Exploration continues until no unexplored vertex is left.