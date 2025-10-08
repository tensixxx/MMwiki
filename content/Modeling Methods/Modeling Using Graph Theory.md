### The Seven Bridges of Königsberg
The Seven Bridges of Königsberg is a famous historical problem, posed in the city of Königsberg (now Kaliningrad, Russia). The city was set on both sides of the Pregel River (shown in the firgue) and included two large islands connected to each other and the mainland by **seven bridges**.
The problem is if it is posssible to walk through all the bridges **exactly** once, starting and ending at the same place.![[Pasted image 20250403133818.png]]
Transforming map in figure above into a **graph**, where every vertex (point) represents a land and every line represents a bridge. 
![[Pasted image 20250403134728.png]]

#### Euler’s Problem (restated)
*Given a graph, under what conditions is it possible to find a closed walk that traverses every edge exactly once?*
Graphs for this kind of walk is possible is called **Eulerian**. The walk is called **Eulerian path**. 
**Conditions for an Eulerian Path**:
1. The graph has to be connected. 
2. The graph has even degree. 

The vertex connects to odd number of lines has **odd degree**; the vertex connects to even number of lines has **even degree**. 

### Graph Coloring
#### Four-Color Problem
Given a geographic map, is it possible to color it with four colors so that any two regions that share a common border (of length greater than 0) are assigned different colors?

![[Pasted image 20250407132247.png]]
The graph above is a United States map with graph, where vertex represents each state and line between two vertices represents the states that share a common border. 
#### Four-Color Problem (restated)
*Using only four colors, can you color the vertices of a graph drawn without edges crossing so that no vertex gets the same color as an adjacent vertex?*
Proved with computer in 1977. Don't have a mathamatical proof until now. 
#### Applications of Graph Coloring
Final exam scheduling problem is an application of graph coloring. 
There are *n* courses and the purpose is to determine the minimize number of exam periods (without conflicts) used. 