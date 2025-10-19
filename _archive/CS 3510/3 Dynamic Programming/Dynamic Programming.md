Fun fact: python functions are all classes. All python functions have state. Because python is evil. 

```python
def f(n):
	if n = 0 return 0
	dp=[0]*n+1
	dp[0]=0
	dp[1]=1
	for i in 2...n:
		dp[i]=dp[i-1]+dp[i-2]
	return dp[n];
```

###### Stair Climbing
Frog can jump 1,2 or 3 steps. How many ways to get up n stairs
```python
def numways(n):
	dp[0...n] all zeroes
	dp[0] = 1
	dp[1] = 1
	dp[2] = 2
	for i in 3...n:
		dp[i]=dp[i-1]+dp[i-2]+dp[i-3]
	return dp[n]
```

###### minimum operations
we can either 
n->n+1
n->n+2
```python
dp[i]=min ops 0 ...i
dp[i]=  i is odd dp[i-1]+1
		i is even min(dp[i/2],dp[i-1]) + 1
```

###### House Robber
rob consecutive cannot rob two in a row 
let $dp[i]$ be max you steal considering houses $h_{1}\dots h_{i}$
```python
dp[i]=max(dp[i-1], dp[i-2]+h_i)
```

###### Lattice Paths

number of lattice paths
$dp[ij,]$ = number of paths to (j,j) from (0,0) = $dp[i-1,j]+dp[i,j-1]$
