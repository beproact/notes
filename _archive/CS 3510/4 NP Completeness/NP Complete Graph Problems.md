Decision SAT is easy $\iff$ search SAT is easy

easily = in polynomial time

Decision Problem says if there is a solution.
Search means you have to find the solution

Descision $\implies$ Search is easy

Search $\implies$ Decision is harder to prove
Use binary search over space.
If we can solve the decision problem easily we can use that to find the actual solution easily.

### INDSET

INDSET = {<G,K> | G have IS of size K?}
set of vertices no two share edge.

3SAT $\leq_{p}$ INDSET

INDSET $\in$ NP

Check witness is exactly k vertices
make sure none of the vertices do not share an edge

#### Reduction
$(\bar{x} \lor y\lor \bar{z})\land(x\lor \bar{y}\lor z)\land(x\lor y\lor z)\land(\bar{x}\lor \bar{y})$
Can turn this into graph

f($\phi$) = <G,k>  G is in the video. k = number clauses.

$\phi\in 3SAT$ The it has some satisfying assignemtn to its K clauses consider
G. By this triangle connection G has an indpendent set of size $\leq$ K.
For each clause of the satisfying assignemtn choose a vertex of the corresponding triangle and add it to a set. Note this is an IS of size k so <a,k> $\in$ IS.

Suppose <G,k> $\in$ IS. Then there is I $\subset$ V of G with |I| = k and no edge shared of the vertices of I. Since G has these K triangles. Exactly one vertex of I is in each triangle. This corresponds to a satisfying assignment of $\phi$ . So $\phi$ is satisfiable.

Also prove the reduction takes polynomial time.

### Clique
CLIQUE = <G,K> | G has a clique of size k

its in NP


INDSET$\leq_{p}$ CLIQUE

if G has an IS of size K $\hat{G}$ has a clique of size k.


### Vertex Cover
Vertex Cover less than size k
Cover every edge

Its in NP.