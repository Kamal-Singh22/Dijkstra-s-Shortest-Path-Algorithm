# Dijkstra-s-Shortest-Path-Algorithm
You are given a weighted graph represented as an adjacency list and a source node. Your task is to calculate the shortest path from the source node to all other nodes in the graph using Dijkstra's Algorithm.
Explanation:
Graph Class: The Graph class stores the adjacency list representation of the graph. Each vertex is a list of Node objects, where each Node represents a neighbor vertex and the weight of the edge connecting them.

addEdge Method: Adds an edge between two vertices with the specified weight. For an undirected graph, edges are added in both directions.

dijkstra Method: The main algorithm. It uses a priority queue (min-heap) to efficiently fetch the vertex with the smallest tentative distance. The dist array tracks the shortest distance from the source to each vertex. If a shorter path is found, it updates the distance and adds the neighbor to the priority queue.

printSolution Method: Prints the shortest distance from the source to every other vertex.

Node Class: Represents each vertex along with its edge weight. The Node class implements the Comparable interface so it can be stored in a priority queue.
