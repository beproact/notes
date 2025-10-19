Pretty much only NP-Hard


$C^*$ optimal 
C output
max($\frac{C}{C^*}$,   $\frac{C^*}{C}$)$\leq \rho(n)$

##### Vertex Cover
```
def AVC(G):
	C=empty
	whiel E to choose:
		choose e=(u,v) in E
		C+=u
		C+=v
		Remove that edge
		
```

AVC is not half bad

Approximation ratio is 2
A be set of edge chosen. Every vertex covers all the subsets of edges
A is covered by every vertex cover.
A is a bunch of disconnected edges
$|C^*|\geq|A|$
$|C|=2|A|\leq2|C^*|$
$\frac{|C|}{|C^*|}\leq2$


##### Set Cover


##### Max 3SAT
Just needs to be expected to approximate to $\rho$

Guess an assignment
