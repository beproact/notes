[[BFS and Dijkstra's]]
Dijkstra's with negative values.
What is a greedy algorithm

$$
\begin{gather}
x \subset T \\
e chosen

\end{gather}
$$

You may not be able to find the optimal solution with a greedy algorithm. You may get stuck at a local minimum.



"Debt isn't real it was made up by capitalists"


update:
dist(v) = min(dist(v), dist(u) + l(u,v))

```python
def bellmanford(G,l,s):
	for all v in V: dist (v) = inf;
	dist(s)= 0
	for i = 1...|V|-1:
		for e = (u,v) in E:
			dist(v) = min(dist(v), min(dist(v), dist(u) + l(u,v)))
```

Runtime of $O(|V|*|E|)$
not good