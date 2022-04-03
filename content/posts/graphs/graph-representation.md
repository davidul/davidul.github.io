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

{{<table `table table-striped table-bordered`>}}
| | 0 | 1 | 2 | 3 |
|-|---|---|---|---|
|0| 0 | 1 | 0 | 1 |
|1| 1 | 0 | 1 | 1 |
|2| 0 | 1 | 0 | 0 |
|3| 1 | 1 | 0 | 0 |
{{</table>}}

This is undirected unweighted graph so we represent every edge by simple 1. Absence of the edge is 0.

Space O(V^2) too much memory needed.

Get all neighbors of a node you have to iterate over the whole row.

## Adjacency list

Stores the edges as linked list. 

``` 
0 | 1 -> 3
1 | 0 -> 2
2 | 1
3 | 0 -> 1
```

The whole datastructure can be stored as list of lists, array of lists, hashmap of lists.

## Edge list
Edges E= {(0,1), (1,2) ...} unweighted
Weighted edges add weight E = {(0,1,5), (1,2,4)}

## Implicit graph

Flood fill. It is a grid, you know (i,j) -> (i-1,j)(i+1,j)(i, j-1)(i,j+1)

## Incidence matrix

