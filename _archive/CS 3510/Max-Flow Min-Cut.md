Flow network.
- Directed graph where each edge has a capacity
- s has no incoming t has no outgoin
Maxflow
What is maximum you can  send from s to t.

Cut
- Partition 
Minimal Cut
- What is lowest number of roads to disconnect s and t


Max flow is the minimum cut

Ford Fulkerson
```python
def FF(G):
	init GF as G
	flow = 0
	while GF has (s-t) path:
		find path
		compute bottleneck
		augment Gf
		flow += b
```

All cuts are more than or equal to every flow.
Where there every edge is saturated there is a cut that is equal to a flow.
# Applications
Edge Disjoint paths
number of edge disjoint paths
Give everything a capacity of 1

People and Jobs
Maximum Matching in a bipartite graph