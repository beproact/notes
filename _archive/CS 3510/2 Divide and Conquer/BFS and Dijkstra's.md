DFS cannot solve Single Source Shortest Path

```python
def BFS(G,S):
	for each v in V:
		dist(v)= inf
	dist(s)=0
	Q=[s]
	while Q!=0:
		u=eject(Q)
		for (u,v) in E:
			if dist(v) = inf
				inject(v) into Q
				dist(v)=dist(u)+1
```
DFS = queue
BFS = stack

Dijkstra's = Priority Queue

PQ: insertion, decrease key, delete min, make queue

```python
def Dijkstra(G,l,s):
	foreach u in V:
		dist(u)=inf
		prev(u)=null
	dist(s)=0
	H= makequeue(dist(v))
	while H != empty:
		u=deletemin(H)
		for(u,v) in E
			if dist(v) > dist(u) +l(u,v)
				dist(u)=dist(u)+l(u,v)
				prev(v)=u
				decreaseKey(h,v) to dist(v)
```

O((V+E)log(v))
Give every node a weight of infinity.
Add every node to two priority queue ordered by their weights, with the lowest weights being at the beginning. We can names these priority queues $$P_p$$ and $$P_q$$
In $$P_p$$ set the weight of p to be 0.
In $$P_q$$ set the weight of q to be 0.
Make a data structure to track if a node has been visited by p or q. We can call these $$V_p$$ and $$V_q$$.

Repeat this until we find the vertex t. Check the min of both $$P_p$$ and $$P_q$$. Find the lowest of these two mins. We can call this "min of mins" m and call the priority queue it came from P. Mark the lowest of the two mins as visited based on whichever priority queue it came from. If it came from $$P_p$$ mark it as visited in $$V_p$$ and if it came from $$P_q$$ mark it as visited in $$V_q$. If it is in the visited of the other visited data structure, our t is the current node we are on and we exit the loop and return it. Next we are going to "eject" the node associated with this lowest of the mins. This means we loop through each edge associated with the min. For each edge we find the sum of the weight of the edge and the weight of our node. If that is lower than the node on the other end of the edge we update that nodes weight to be the sum we found. 