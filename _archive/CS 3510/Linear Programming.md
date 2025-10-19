Set of linear equations

Must be linear.
Can be turned into matrices


2 Features of Linear Programming

Polytope- Shape Find solutions in the polytope
Solution always occurs on an exterior point
Always convex.


No solution
infeasable
unbounded

Simplex - Greedy
Walk on exterior towards exterior points that moves towards the goal.
At a very high level
```python
begin at v= (0,0)
while True:
	if for any v' neighbor of v more optimal
		v=v'
	else break
```

Simplex and Duality

There are finitely many points to check.

First add slack variables
