+++
author = "David Ulicny"
title = "Graph Representation"
date = "2022-03-04"
description = "How to represent a graph"
tags = [
    "graph",
    "algorithm",
]
categories = [
    "graphs",
    "algorithms",
]
series = ["Graphs"]
+++

# Graph representation
Types of graph:
* Undirected graph
* Directed graph
* Weighted graph 

## Adjacency matrix

Adjacency matrix stores the edges in a matrix. Adjacency matrix for this graph
would be

![Example graph](../../slice1.png "graph")

| | 0 | 1 | 2 | 3 |
|-|---|---|---|---|
|0| 0 | 1 | 0 | 1 |
|1| 1 | 0 | 1 | 1 |
|2| 0 | 1 | 0 | 0 |
|3| 1 | 1 | 0 | 0 |

This is undirected unweighted graph so we represent every edge by simple 1. Absence of the edge is 0.

## Adjacency list

Stores the edges as linked list. 

``` 
0 | 1 -> 3
1 | 0 -> 2
2 | 1
3 | 0 -> 1
```


## Incidence matrix
