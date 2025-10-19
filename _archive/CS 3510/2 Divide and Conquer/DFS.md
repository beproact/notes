Depth First Search
Graphs - Sequence of points connect by lines.
$$
\begin{gather}
G=(V,E) \\
V=\{v_{1}\dots vk\} \\
E \subseteq V\times V
\end{gather}
$$
Graph is topological. Position does not matter. Relationship matters.

###### How to encode graphs
Adjacency Matrix- Stores too much irrelevant data.
Graphs is dense if a lot of edges.
Graph is sparse if few edges.
Most graphs are sparse
$|E|$ usually ranges between $|V|$ and $|V|^2$

Adjacency List
List for each vertex with the list of connections.

```python
def explore(G,v):
	marked[v]=true
	previsit(v)
	for edge(v,u) in E:
		if(not marked[v]):
		explore(u)
	postvisit(v)

def DFS(G):
	for v in V:
		marked[v]=false
	for v in V:
		if not marked[v]:
			explore(G,v)

def previsit(v):
	pre[v] = counter
	counter++
def postvisit(v):
	post[v] = counter
	counter++
```
O(V+E)

Cycle Detection
Directed Acyclic Graph
think posets
Can figure out if graph is a DAG using DFS
```python
def cycleDetect(G,V):
	marked[v]=true
	tempmark[v]=true #pre
	for(v,u) in E:
		if tempmarked[v]: print "cycle"
		if not marked[v]:
			explore(G,u)
	tempmark[v]=false #post
```
O(V+E)

Topological Sort/ Linearization

```python
def topsort(G,V):
	marked[v]=true
	for(v,u) in E
		if no marked[u]:
			explore(G,V)
	L=[v]++L #appends v to front
```


Strongly Connected Component if path both ways.
Smallest connect component is a a cycle
Metagraph is a DAG.

C->C'
The highest postlabel of C > the highest postlabel of C'

Exploring a sink of the metagraph touches only that component

Graph reversal- Take every edge and reverse it
sources of the reversal are sinks of the original 

```python
def SCC(G):
	computer G^R
	DFS on GR get post labels in decreasing order
	while posts is not empty:
		v=max(posts)
		comp = explore(G,v)
		mark and delete comp from G posts
```
O(V+E)

