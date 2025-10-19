#### Polytime Reduction
$A\leq_{p}B$ if there is a function F computable in polytime such that $x \in A \iff f(x)\in B$
If B is easy A is easy
If A is hard then B is hard
"B is harder than A"


B is NP-complete if 
1. $B\in NP$
2. $\forall A\in N, A\leq_{p}B$ (NP hard)

#### Sat
variable $x,y,z$ 
literal $x,y,z\dots,\lnot x\dots$
Clause is or of literals
CNF is and of clauses
SAT = {<$\Phi$> | $\Phi$ has a satisfying assignment}

To verify just plug in.
You can't easily verify SAT does not have satisfying assignment

##### 3SAT
Same as SAT and each clause has at most 3 literals
NP complete
let a clause be $(x_{1}\lor x_{2}\lor x_{3}\dots \lor x_{k})$ for $k\geq4$

#### Circuit SAT
n inputs 1 output
some input exists to make the output 1

3SAT $\leq_{p}$ circuitSAT