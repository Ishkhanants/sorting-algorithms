Breadth First Traversal (or Search) for a graph is similar to Breadth First Traversal of a tree (See method 2 of this post). The only catch here is, unlike trees, graphs may contain cycles, so we may come to the same node again. To avoid processing a node more than once, we use a boolean visited array. For simplicity, it is assumed that all vertices are reachable from the starting vertex.

For example, in the following graph, we start traversal from vertex 2. When we come to vertex 0, we look for all adjacent vertices of it. 2 is also an adjacent vertex of 0. If we don’t mark visited vertices, then 2 will be processed again and it will become a non-terminating process. A Breadth First Traversal of the following graph is 2, 0, 3, 1.

![img.png](infoimgs/img.png)

![img_1.png](infoimgs/img_1.png)
![img_2.png](infoimgs/img_2.png)
![img_3.png](infoimgs/img_3.png)
![img_4.png](infoimgs/img_4.png)
![img_5.png](infoimgs/img_5.png)
