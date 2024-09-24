---
{"dg-publish":true,"permalink":"/Mainfolder/IBDP-Mathematics/Introduction to sequence/"}
---

- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Definition of a Sequence\|Definition of a Sequence]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Definition of a Sequence\|Example:]]
- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Notation and Examples of Sequences\|Notation and Examples of Sequences]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Notation and Examples of Sequences\|Notation:]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Notation and Examples of Sequences\|Examples:]]
		- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Examples:\|1. Constant Sequence:]]
		- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Examples:\|2. Arithmetic Sequence:]]
		- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Examples:\|3. Geometric Sequence:]]
		- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Examples:\|4. Harmonic Sequence:]]
- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Convergence and Divergence of Sequences\|Convergence and Divergence of Sequences]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Convergence and Divergence of Sequences\|Convergence:]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Convergence and Divergence of Sequences\|Divergence:]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Convergence and Divergence of Sequences\|Example of Convergence:]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Convergence and Divergence of Sequences\|Example of Divergence:]]
- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Limits of Sequences\|Limits of Sequences]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Limits of Sequences\|Formal Definition:]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Limits of Sequences\|Limit Laws for Sequences:]]
- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Bounded and Monotonic Sequences\|Bounded and Monotonic Sequences]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Bounded and Monotonic Sequences\|Bounded Sequences:]]
		- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Bounded Sequences:\|Example of a Bounded Sequence:]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Bounded and Monotonic Sequences\|Monotonic Sequences:]]
		- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Monotonic Sequences:\|Example of a Monotonically Increasing Sequence:]]
		- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Monotonic Sequences:\|Example of a Monotonically Decreasing Sequence:]]
	- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#Bounded and Monotonic Sequences\|The Monotone Convergence Theorem:]]
		- [[Mainfolder/IBDP-Mathematics/Introduction to sequence#The Monotone Convergence Theorem:\|Example:]]

## Definition of a Sequence
- A **sequence** is an ordered list of numbers, often defined as a function whose domain is the set of natural numbers. Each number in the list is called a **term** of the sequence.
  
- Formally, a sequence is a function $f: \mathbb{N} \to \mathbb{R}$, where $\mathbb{N}$ is the set of natural numbers and $\mathbb{R}$ is the set of real numbers. The value of the function $f$ at a natural number $n$ is called the $n$-th term of the sequence and is typically denoted by $a_n$.

### Example:
If $a_n = \frac{1}{n}$, the sequence is:
$$
a_1 = 1, a_2 = \frac{1}{2}, a_3 = \frac{1}{3}, \dots
$$
This gives the sequence:
$$
\left(1, \frac{1}{2}, \frac{1}{3}, \frac{1}{4}, \dots \right)
$$

---

## Notation and Examples of Sequences

### Notation:
A sequence is typically written in one of the following forms:
- $\{a_n\}_{n=1}^{\infty}$: A sequence where the $n$-th term is $a_n$.
- $(a_n)_{n=1}^{\infty}$: Another common notation for sequences.
  
The **general term** of the sequence is given by a formula $a_n$, which determines the value of each term based on $n$.

### Examples:

#### 1. Constant Sequence:
A sequence where every term is the same, such as $a_n = c$ for all $n \in \mathbb{N}$.
- Example: $a_n = 5$, giving the sequence $(5, 5, 5, 5, \dots)$.

#### 2. Arithmetic Sequence:
A sequence where each term is the previous term plus a constant difference $d$.
- Example: $a_n = 2n$, giving the sequence $(2, 4, 6, 8, \dots)$.

#### 3. Geometric Sequence:
A sequence where each term is the previous term multiplied by a constant ratio $r$.
- Example: $a_n = 3 \cdot 2^n$, giving the sequence $(6, 12, 24, 48, \dots)$.

#### 4. Harmonic Sequence:
A sequence where each term is the reciprocal of an arithmetic sequence.
- Example: $a_n = \frac{1}{n}$, giving the sequence $\left(1, \frac{1}{2}, \frac{1}{3}, \dots \right)$.

---

## Convergence and Divergence of Sequences

### Convergence:
A sequence $\{a_n\}$ **converges** to a real number $L$ if, as $n$ becomes very large, the terms of the sequence get arbitrarily close to $L$. More formally, $\{a_n\}$ converges to $L$ if for every $\epsilon > 0$, there exists a natural number $N$ such that for all $n > N$, we have:
$$
|a_n - L| < \epsilon
$$
In this case, we write:
$$
\lim_{n \to \infty} a_n = L \quad \text{or} \quad a_n \to L \text{ as } n \to \infty
$$

### Divergence:
If a sequence does not converge to a finite limit, we say that it **diverges**. A sequence can diverge in various ways:
- **Divergence to infinity**: The terms of the sequence grow without bound as $n$ increases.
  - Example: The sequence $a_n = n$ diverges to infinity as $n \to \infty$.
  
- **Oscillatory divergence**: The terms of the sequence oscillate between values without approaching a single limit.
  - Example: The sequence $a_n = (-1)^n$ oscillates between $1$ and $-1$ and does not converge.

### Example of Convergence:
The sequence $a_n = \frac{1}{n}$ converges to $0$:
$$
\lim_{n \to \infty} \frac{1}{n} = 0
$$

### Example of Divergence:
The sequence $a_n = n$ diverges to infinity:
$$
\lim_{n \to \infty} n = \infty
$$

---

## Limits of Sequences

The **limit** of a sequence describes the value (if any) that the terms of the sequence approach as $n$ increases without bound.

### Formal Definition:
The sequence $\{a_n\}$ has a limit $L$ if for every $\epsilon > 0$, there exists an integer $N$ such that for all $n > N$:
$$
|a_n - L| < \epsilon
$$
This definition formalizes the idea that beyond some index $N$, the terms of the sequence are all within a small distance $\epsilon$ of $L$.

### Limit Laws for Sequences:
If $\lim_{n \to \infty} a_n = L$ and $\lim_{n \to \infty} b_n = M$, then:
1. **Sum Rule**: $\lim_{n \to \infty} (a_n + b_n) = L + M$
2. **Difference Rule**: $\lim_{n \to \infty} (a_n - b_n) = L - M$
3. **Product Rule**: $\lim_{n \to \infty} (a_n \cdot b_n) = L \cdot M$
4. **Quotient Rule**: $\lim_{n \to \infty} \frac{a_n}{b_n} = \frac{L}{M}$, provided $M \neq 0$

---

## Bounded and Monotonic Sequences

### Bounded Sequences:
A sequence $\{a_n\}$ is called **bounded** if there exists a real number $M$ such that for all $n$, $|a_n| \leq M$. In other words, the terms of the sequence stay within a fixed range.

- A sequence is **bounded above** if there exists an $M$ such that $a_n \leq M$ for all $n$.
- A sequence is **bounded below** if there exists an $m$ such that $a_n \geq m$ for all $n$.

#### Example of a Bounded Sequence:
The sequence $a_n = \frac{1}{n}$ is bounded since $0 \leq a_n \leq 1$ for all $n$.

### Monotonic Sequences:
A sequence $\{a_n\}$ is **monotonic** if its terms are always increasing or always decreasing.

- A sequence is **monotonically increasing** if $a_n \leq a_{n+1}$ for all $n$.
- A sequence is **monotonically decreasing** if $a_n \geq a_{n+1}$ for all $n$.

#### Example of a Monotonically Increasing Sequence:
The sequence $a_n = n$ is monotonically increasing since $a_n \leq a_{n+1}$ for all $n$.

#### Example of a Monotonically Decreasing Sequence:
The sequence $a_n = \frac{1}{n}$ is monotonically decreasing since $a_n \geq a_{n+1}$ for all $n$.

### The Monotone Convergence Theorem:
If a sequence is both **monotonic** and **bounded**, then it **converges**.

#### Example:
The sequence $a_n = \frac{1}{n}$ is both monotonically decreasing and bounded below by $0$, so by the monotone convergence theorem, it converges to $0$:
$$
\lim_{n \to \infty} \frac{1}{n} = 0
$$
