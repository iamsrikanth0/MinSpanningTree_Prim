# MinSpanningTree_Prim
What is MST? 1. Includes all Nodes 2. Min edge weight 3. No cycle (that is why it is called Tree)--->> Only for Undirected graphs
We prim's algo- MST set and Non MST set, here we will start with one starting point, Node, push it to MST set, now we will check which one has low weight and then start pushing the second one. We will check all the neighbours whose cost/wt is low , then push to MST. This is the approach.
So here we are expecting to get min wt node, this can be done by Priority Queue. There in Code, our Non MST is nothing but a priority Queue. Role of MST set is done by Visited array
