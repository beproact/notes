Shortest paths in DAGs


Single Source Shortest Path

```python
def SSSPDAG(G,l,S):
	for all v in V: dist(v)=inf
	dist(s)=0
	TopSort G
	for u in V:(in top sort order)
		for(u,v) in E:
			dist(v) = min(dist(v),dist(u)+l(u,v))
```

O(V+E)
We know there is no path going backwards in the topsort



Floyd Warshall uses dynamic programming to calculate best paths for every node.
prob rewatch this


