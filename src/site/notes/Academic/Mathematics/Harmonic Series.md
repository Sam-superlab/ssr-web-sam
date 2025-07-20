---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Harmonic Series/"}
---

- [[Academic/Mathematics/Harmonic Series#Definition of the Harmonic Series\|Definition of the Harmonic Series]]
	- [[Academic/Mathematics/Harmonic Series#Definition of the Harmonic Series\|Example:]]
- [[Academic/Mathematics/Harmonic Series#Divergence of the Harmonic Series\|Divergence of the Harmonic Series]]
	- [[Academic/Mathematics/Harmonic Series#Divergence of the Harmonic Series\|Proof of Divergence:]]
- [[Academic/Mathematics/Harmonic Series#Comparison with $p$-Series\|Comparison with $p$-Series]]
	- [[Academic/Mathematics/Harmonic Series#Comparison with $p$-Series\|Convergence and Divergence of $p$-Series:]]
	- [[Academic/Mathematics/Harmonic Series#Comparison with $p$-Series\|Comparison Example:]]

## Definition of the Harmonic Series

A **harmonic series** is a specific type of infinite series where each term is the reciprocal of a positive integer. The harmonic series is given by:
$$
S = \sum_{n=1}^{\infty} \frac{1}{n} = 1 + \frac{1}{2} + \frac{1}{3} + \frac{1}{4} + \dots
$$
Each term $a_n = \frac{1}{n}$ decreases as $n$ increases, but the terms decrease very slowly compared to other series.

### Example:
The sum of the first few terms of the harmonic series is:
$$
S_4 = 1 + \frac{1}{2} + \frac{1}{3} + \frac{1}{4} = 2.0833
$$
Even though the terms get smaller, the sum keeps increasing as more terms are added.

---

## Divergence of the Harmonic Series

Despite the fact that the terms of the harmonic series get smaller and smaller, the harmonic series **diverges**. This means that as you keep adding more and more terms, the sum grows without bound.

### Proof of Divergence:

One way to show that the harmonic series diverges is by grouping terms and comparing them to a series that grows without bound.

Consider:
$$
S = 1 + \frac{1}{2} + \left( \frac{1}{3} + \frac{1}{4} \right) + \left( \frac{1}{5} + \frac{1}{6} + \frac{1}{7} + \frac{1}{8} \right) + \dots
$$
Group the terms as follows:
- The first group has 1 term: $1$.
- The second group has 1 term: $\frac{1}{2}$.
- The third group has 2 terms: $\frac{1}{3} + \frac{1}{4}$, and each term is greater than or equal to $\frac{1}{4}$.
- The fourth group has 4 terms: $\frac{1}{5} + \frac{1}{6} + \frac{1}{7} + \frac{1}{8}$, and each term is greater than or equal to $\frac{1}{8}$.

For each group of terms, the total contribution is greater than or equal to $\frac{1}{2}$. Since there are infinitely many such groups, the total sum of the series grows without bound, proving that the harmonic series diverges.

Thus, we conclude:
$$
\sum_{n=1}^{\infty} \frac{1}{n} = \infty
$$

---

## Comparison with $p$-Series

The harmonic series is a special case of the **$p$-series**, which has the general form:
$$
\sum_{n=1}^{\infty} \frac{1}{n^p}
$$
Where $p$ is a constant.

### Convergence and Divergence of $p$-Series:
- The $p$-series converges if $p > 1$.
- The $p$-series diverges if $p \leq 1$.

The harmonic series is the case when $p = 1$, and as we’ve seen, it **diverges**:
$$
\sum_{n=1}^{\infty} \frac{1}{n} \quad \text{(diverges)}
$$

### Comparison Example:
- For $p = 2$, we have the **convergent** series:
$$
\sum_{n=1}^{\infty} \frac{1}{n^2} = 1 + \frac{1}{4} + \frac{1}{9} + \frac{1}{16} + \dots
$$
This series converges to a finite value, specifically $\frac{\pi^2}{6}$ (a result from Euler).

- For $p = \frac{1}{2}$, we have the **divergent** series:
$$
\sum_{n=1}^{\infty} \frac{1}{n^{\frac{1}{2}}} = 1 + \frac{1}{\sqrt{2}} + \frac{1}{\sqrt{3}} + \dots
$$
This series diverges because $p \leq 1$.
