# MinSpanningTree_Prim
What is MST? 1. Includes all Nodes 2. Min edge weight 3. No cycle (that is why it is called Tree)--->> Only for Undirected graphs
We prim's algo- MST set and Non MST set, here we will start with one starting point, Node, push it to MST set, now we will check which one has low weight and then start pushing the second one. We will check all the neighbours whose cost/wt is low , then push to MST. This is the approach.
So here we are expecting to get min wt node, this can be done by Priority Queue. There in Code, our Non MST is nothing but a priority Queue. Role of MST set is done by Visited array
Worst Case- we will have to add all the edges, so O(ElogE)
Dry run the code for clear understanding. 
We didn't do any relaxation here, we just used the property of PQ and visited array and got min distance, all nodes being connected. Seems like an alternative to dijkstra algorithm. 
Main difference between Dijkstra algorithm and this prim's is, Dijkstra gives minimum distance from starting node to each other node. whereas prim's gives minimum distance of the total edge weight of the tree that connects all nodes. PQ can only give the min from nrighbours, but it cannot give other routes distances, for this we use relaxation. Using relaxation is important
The core difference is path vs tree. MST gives you a tree, it covers all the nodes with minimum total edge weight, but it does not gaurantee the Shortest path from the source to all other Nodes. 
