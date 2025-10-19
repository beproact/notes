Chain Matrix multiplication
Partition DP

Depending on order you do matrix multiplication orders in the amount of steps changes.

You have to consider 

$$
\begin{gather}
(A)(A_{2}\dots A_{n}) \\
(AA_{2})(A_{3}\dots A_{n}) \\
. \\
. \\
. \\
(A\dots A_{n-1})(A_{n})
\end{gather}
$$

```python
dp[i,j]=min(i<=k<j) (dp[i,k] + dp[k+1,j]+d(i-1)+dk+dj)
```
