# Dijkstra-s-Shortest-Path-Algorithm
You are given a weighted graph represented as an adjacency list and a source node. Your task is to calculate the shortest path from the source node to all other nodes in the graph using Dijkstra's Algorithm.


Input:
An integer 𝑛, representing the number of nodes in the graph.
An integer 𝑚, representing the number of edges.
A list of 𝑚 edges, where each edge is described as (𝑢,𝑣,𝑤)(u,v,w).
An integer 𝑠s, the source node from which to calculate the shortest paths.



Explanation:
From the top-left corner, the robot can:
Go down, down, right.
Go down, right, down.
Go right, down, down.
Constraints:
1≤𝑚,𝑛≤100 1≤m,n≤100
The answer is guaranteed to be within the range of a 32-bit integer.


Explanation:
Graph Class: The Graph class stores the adjacency list representation of the graph. Each vertex is a list of Node objects, where each Node represents a neighbor vertex and the weight of the edge connecting them.

addEdge Method: Adds an edge between two vertices with the specified weight. For an undirected graph, edges are added in both directions.

dijkstra Method: The main algorithm. It uses a priority queue (min-heap) to efficiently fetch the vertex with the smallest tentative distance. The dist array tracks the shortest distance from the source to each vertex. If a shorter path is found, it updates the distance and adds the neighbor to the priority queue.

printSolution Method: Prints the shortest distance from the source to every other vertex.

Node Class: Represents each vertex along with its edge weight. The Node class implements the Comparable interface so it can be stored in a priority queue.
