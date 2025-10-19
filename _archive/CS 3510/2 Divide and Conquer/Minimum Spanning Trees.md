Minimum Spanning Tree
Kruskal's is a greedy algorithm. Keep adding lightest edge that does not make a cycle.
```python
def Kruskals(G=(V,E)):
	sort E by weight
	T={}
	for e=(u,v) in E:
		if T+e contains cycles
			skip
		else T=T+e
```
Union Find
Puts things into partitions.
Find: returns set with in v in it
union: takes two disjoints sets combines them