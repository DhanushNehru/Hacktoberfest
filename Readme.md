# Dijkstra's Algorithm in Python

This Python script implements **Dijkstra's Algorithm** to find the shortest paths from a source vertex in a weighted graph with non-negative edge weights.

## How It Works

1. Set the distance to the source vertex as 0, all others as infinity.
2. Use a min-heap to select the vertex with the smallest known distance.
3. For each neighbor, update the distance if a shorter path is found.
4. Repeat until all vertices are processed.

## Getting Started

### Prerequisites

Ensure Python is installed. [Download here](https://www.python.org/downloads/).

### Running the Script

1. Clone the repository.
2. Run the script using:

   ```bash
   python dijkstra.py
   
INPUT FORMAT

The input consists of:

* Number of vertices: Enter the total number of vertices in the graph.
* Graph representation:
      For each vertex:
    * Input the vertex name.
    * Enter the number of edges connected to that vertex.
    * For each edge, input the neighboring vertex and the edge weight, separated by a space.
* Source vertex: Enter the name of the source vertex from which the shortest paths will be calculated.

example: 

<pre>
Enter number of vertices: 4
Enter vertex: A
Enter number of edges for A: 2
Enter neighbor and weight separated by space: B 1
Enter neighbor and weight separated by space: C 4
Enter vertex: B
Enter number of edges for B: 3
Enter neighbor and weight separated by space: A 1
Enter neighbor and weight separated by space: C 2
Enter neighbor and weight separated by space: D 5
Enter vertex: C
Enter number of edges for C: 3
Enter neighbor and weight separated by space: A 4
Enter neighbor and weight separated by space: B 2
Enter neighbor and weight separated by space: D 1
Enter vertex: D
Enter number of edges for D: 2
Enter neighbor and weight separated by space: B 5
Enter neighbor and weight separated by space: C 1
Enter the source vertex: A
</pre>


4: Number of vertices in the graph.
A, B, C, D: The vertices of the graph.
B 1, C 4: Vertex A has edges to B with weight 1, and to C with weight 4.
A: The source vertex for shortest path calculations.

OUTPUT FORMAT
Shortest distances from A: {'A': 0, 'B': 1, 'C': 3, 'D': 4}