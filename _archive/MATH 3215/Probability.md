#### Kolmogorov Axioms
We say a real-valued set function $\mathbb{P}(\cdot)$ is a probability measure if
- $P(A)\geq 0$ for any event $A$
- $P(\Omega)=1$ where $\Omega$ is the sample space.
- For mutually exclusive events $E_{1},E_{2},E_{3}\dots$
$$
\mathbb{P}\left( \cup_{i=1}^{\infty}E_{i}=\sum_{i=1}^{\infty}\mathbb{P}(E_{i}) \right)
$$

#### Common Probability Properties
- Set Subtraction
	- $\mathbb{P}(A\setminus B)=\mathbb{P}(A)-\mathbb{P}(A \cap B)$
- Complement
	- $\mathbb{P}(A^C)=1-\mathbb{P}(A)$
- Inclusion exclusion
	- $\mathbb{P}(A\cup B)=\mathbb{P}(A)+\mathbb{P}(B)-\mathbb{P}(A\cap B)$
- If $A\subseteq B$, then
	- $\mathbb{P}(A)\leq \mathbb{P}(B)$

#### Equally likely outcome model
- Let $\Omega =\{\omega_{1},\omega_{2},\omega_{3},\dots,\omega_{n}\}$ be the sample space of some random experiment with finite (n) outcomes. If probability of each is equal then.
$$
\mathbb{P}(\{\omega_{i}\})=\frac{1}{n}
$$
$$
\mathbb{P}(E_{1})=\frac{{|E_{1}|}}{|\Omega|}
$$
#### Conditional Probability
$$\mathbb{P}(A|B)=\frac{{\mathbb{P}(A\cap B)}}{\mathbb{P}(B)}$$
#### Probability Product Rule
$$
\begin{gather}
\mathbb{P}(A \cap B)=\mathbb{P}(A|B) \mathbb{P}(B)=\mathbb{P}(B|A)\mathbb{P}(A) \\
P(A|B)=\frac{{\mathbb{P}(B|A)P(A)}}{\mathbb{P}(B)}
\end{gather}
$$
usually 2nd event | 1st event
2nd event given 1st event

#### Partition