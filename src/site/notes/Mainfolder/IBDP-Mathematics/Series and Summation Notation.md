---
{"dg-publish":true,"permalink":"/Mainfolder/IBDP-Mathematics/Series and Summation Notation/"}
---

- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Definition of a Series\|Definition of a Series]]
- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Summation Notation (Sigma Notation)\|Summation Notation (Sigma Notation)]]
	- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Summation Notation (Sigma Notation)\|Example:]]
- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Partial Sums\|Partial Sums]]
	- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Partial Sums\|Example of Partial Sums:]]
- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Infinite Series\|Infinite Series]]
- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Convergence and Divergence of Series\|Convergence and Divergence of Series]]
	- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Convergence and Divergence of Series\|Convergence:]]
	- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Convergence and Divergence of Series\|Example of a Convergent Series:]]
	- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Convergence and Divergence of Series\|Divergence:]]
	- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Convergence and Divergence of Series\|Example of a Divergent Series:]]
	- [[Mainfolder/IBDP-Mathematics/Series and Summation Notation#Convergence and Divergence of Series\|Tests for Convergence:]]

## Definition of a Series
A **series** is the sum of the terms of a sequence. If $\{a_n\}$ is a sequence, then the corresponding series is written as:
$$
S = a_1 + a_2 + a_3 + \dots
$$
More generally, the sum of the first $n$ terms of a sequence is called the **partial sum** of the series:
$$
S_n = a_1 + a_2 + \dots + a_n = \sum_{k=1}^{n} a_k
$$
A series can either be **finite** (a sum of a fixed number of terms) or **infinite** (a sum of infinitely many terms). 

---

## Summation Notation (Sigma Notation)
**Summation notation** (also called **sigma notation**) is a compact way of writing the sum of the terms in a sequence. It is represented using the Greek capital letter $\Sigma$:
$$
\sum_{k=1}^{n} a_k
$$
Where:
- $\Sigma$ represents summation.
- $k$ is the **index of summation**, typically starting at 1.
- $n$ is the **upper limit**, indicating how many terms to sum.
- $a_k$ represents the $k$-th term of the sequence.

### Example:
The sum of the first $5$ terms of the sequence $a_n = n^2$ can be written as:
$$
\sum_{n=1}^{5} n^2 = 1^2 + 2^2 + 3^2 + 4^2 + 5^2 = 1 + 4 + 9 + 16 + 25 = 55
$$

---

## Partial Sums
A **partial sum** is the sum of the first $n$ terms of a series. The partial sum of the series $\{a_n\}$ is given by:
$$
S_n = a_1 + a_2 + a_3 + \dots + a_n = \sum_{k=1}^{n} a_k
$$
Partial sums are important because they help analyze whether an **infinite series** converges or diverges.

### Example of Partial Sums:
For the sequence $a_n = \frac{1}{n}$, the partial sums for the first 3 terms are:
$$
S_1 = 1, \quad S_2 = 1 + \frac{1}{2} = \frac{3}{2}, \quad S_3 = 1 + \frac{1}{2} + \frac{1}{3} = \frac{11}{6}
$$

---

## Infinite Series
An **infinite series** is the sum of infinitely many terms of a sequence:
$$
S = a_1 + a_2 + a_3 + \dots = \sum_{k=1}^{\infty} a_k
$$
The sum of an infinite series is defined as the **limit** of the sequence of partial sums. If the partial sums approach a finite number $S$, we say the series **converges** to $S$:
$$
S = \lim_{n \to \infty} S_n
$$
If the partial sums do not approach a finite limit, we say the series **diverges**.

---

## Convergence and Divergence of Series

### Convergence:
An infinite series $\sum_{n=1}^{\infty} a_n$ **converges** if the sequence of partial sums $\{S_n\}$ has a finite limit as $n \to \infty$. That is:
$$
\lim_{n \to \infty} S_n = L
$$
where $L$ is a real number. The series then sums to $L$.

### Example of a Convergent Series:
Consider the geometric series:
$$
S = 1 + \frac{1}{2} + \frac{1}{4} + \frac{1}{8} + \dots
$$
This series converges to:
$$
S = \frac{1}{1 - \frac{1}{2}} = 2
$$

### Divergence:
An infinite series $\sum_{n=1}^{\infty} a_n$ **diverges** if the partial sums do not approach a finite limit. This may happen if the partial sums grow without bound, or if they oscillate between values without settling on a single number.

### Example of a Divergent Series:
The harmonic series $\sum_{n=1}^{\infty} \frac{1}{n}$ is an example of a divergent series:
$$
S = 1 + \frac{1}{2} + \frac{1}{3} + \frac{1}{4} + \dots
$$
Although the terms get smaller, the partial sums increase without bound, meaning the series diverges.

### Tests for Convergence:
There are several tests to determine if a series converges or diverges, including:
1. **nth-Term Test for Divergence**: If $\lim_{n \to \infty} a_n \neq 0$, then the series diverges.
2. **Geometric Series Test**: A geometric series $\sum_{n=0}^{\infty} ar^n$ converges if $|r| < 1$.
3. **Integral Test**: A series $\sum a_n$ can be compared to an integral $\int f(x) dx$ to test for convergence.
4. **Comparison Test**: Compare the series $\sum a_n$ with another known convergent or divergent series to determine the behavior.
