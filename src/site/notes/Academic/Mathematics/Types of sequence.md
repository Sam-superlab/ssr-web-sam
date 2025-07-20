---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Types of sequence/"}
---

- [[Academic/Mathematics/Types of sequence#Arithmetic Sequences\|Arithmetic Sequences]]
	- [[Academic/Mathematics/Types of sequence#Arithmetic Sequences\|Definition:]]
	- [[Academic/Mathematics/Types of sequence#Arithmetic Sequences\|Example:]]
	- [[Academic/Mathematics/Types of sequence#Arithmetic Sequences\|Sum of an Arithmetic Sequence:]]
- [[Academic/Mathematics/Types of sequence#Geometric Sequences\|Geometric Sequences]]
	- [[Academic/Mathematics/Types of sequence#Geometric Sequences\|Definition:]]
	- [[Academic/Mathematics/Types of sequence#Geometric Sequences\|Example:]]
	- [[Academic/Mathematics/Types of sequence#Geometric Sequences\|Sum of a Geometric Sequence:]]
- [[Academic/Mathematics/Types of sequence#Harmonic Sequences\|Harmonic Sequences]]
	- [[Academic/Mathematics/Types of sequence#Harmonic Sequences\|Definition:]]
	- [[Academic/Mathematics/Types of sequence#Harmonic Sequences\|Example:]]
	- [[Academic/Mathematics/Types of sequence#Harmonic Sequences\|Harmonic Series:]]
- [[Academic/Mathematics/Types of sequence#Recursive Sequences\|Recursive Sequences]]
	- [[Academic/Mathematics/Types of sequence#Recursive Sequences\|Definition:]]
	- [[Academic/Mathematics/Types of sequence#Recursive Sequences\|Example:]]
	- [[Academic/Mathematics/Types of sequence#Recursive Sequences\|General Recursive Formula:]]
		- [[Academic/Mathematics/Types of sequence#General Recursive Formula:\|Example (Geometric Recursive):]]
- [[Academic/Mathematics/Types of sequence#Fibonacci Sequence\|Fibonacci Sequence]]
	- [[Academic/Mathematics/Types of sequence#Fibonacci Sequence\|Definition:]]
	- [[Academic/Mathematics/Types of sequence#Fibonacci Sequence\|Properties of the Fibonacci Sequence:]]


## Arithmetic Sequences

### Definition:
An **arithmetic sequence** is a sequence in which each term is obtained by adding a constant difference $d$ to the previous term. The general form of an arithmetic sequence is:
$$
a_n = a_1 + (n - 1)d
$$
where:
- $a_n$ is the $n$-th term.
- $a_1$ is the first term.
- $d$ is the common difference between consecutive terms.

### Example:
Consider the arithmetic sequence with $a_1 = 3$ and $d = 2$. The sequence is:
$$
3, 5, 7, 9, 11, \dots
$$
Using the formula for the $n$-th term:
$$
a_n = 3 + (n - 1) \cdot 2 = 2n + 1
$$

### Sum of an Arithmetic Sequence:
The sum of the first $n$ terms of an arithmetic sequence (arithmetic series) is given by:
$$
S_n = \frac{n}{2} \cdot (a_1 + a_n)
$$
or equivalently:
$$
S_n = \frac{n}{2} \cdot (2a_1 + (n - 1)d)
$$

---

## Geometric Sequences

### Definition:
A **geometric sequence** is a sequence in which each term is obtained by multiplying the previous term by a constant ratio $r$. The general form of a geometric sequence is:
$$
a_n = a_1 \cdot r^{n-1}
$$
where:
- $a_n$ is the $n$-th term.
- $a_1$ is the first term.
- $r$ is the common ratio between consecutive terms.

### Example:
Consider the geometric sequence with $a_1 = 2$ and $r = 3$. The sequence is:
$$
2, 6, 18, 54, 162, \dots
$$
Using the formula for the $n$-th term:
$$
a_n = 2 \cdot 3^{n-1}
$$

### Sum of a Geometric Sequence:
The sum of the first $n$ terms of a geometric sequence (geometric series) is given by:
$$
S_n = a_1 \cdot \frac{1 - r^n}{1 - r}, \quad r \neq 1
$$
The sum of an infinite geometric series is:
$$
S = \frac{a_1}{1 - r}, \quad |r| < 1
$$

---

## Harmonic Sequences

### Definition:
A **harmonic sequence** is a sequence where each term is the reciprocal of the corresponding term in an arithmetic sequence. The general form of a harmonic sequence is:
$$
a_n = \frac{1}{n}
$$
or, more generally:
$$
a_n = \frac{1}{a_1 + (n-1)d}
$$
where $a_1$ is the first term and $d$ is the common difference of the corresponding arithmetic sequence.

### Example:
The harmonic sequence corresponding to the arithmetic sequence $1, 2, 3, 4, \dots$ is:
$$
1, \frac{1}{2}, \frac{1}{3}, \frac{1}{4}, \dots
$$

### Harmonic Series:
The sum of the harmonic sequence (the harmonic series) is:
$$
\sum_{n=1}^{\infty} \frac{1}{n} = 1 + \frac{1}{2} + \frac{1}{3} + \dots
$$
This series **diverges**, meaning it grows without bound as more terms are added, even though each term gets smaller.

---

## Recursive Sequences

### Definition:
A **recursive sequence** is defined by a recurrence relation, where each term is a function of one or more of the previous terms. Instead of providing an explicit formula for $a_n$, a recursive sequence gives a relationship between $a_n$ and previous terms like $a_{n-1}$, $a_{n-2}$, etc.

### Example:
The sequence defined by the recurrence relation:
$$
a_n = a_{n-1} + 2, \quad a_1 = 3
$$
is a recursive arithmetic sequence where each term is the previous term plus 2. The sequence is:
$$
3, 5, 7, 9, 11, \dots
$$

### General Recursive Formula:
Many recursive sequences are defined in terms of both initial conditions and a recursive formula.

#### Example (Geometric Recursive):
$$
a_n = r \cdot a_{n-1}, \quad a_1 = 2
$$
With $r = 3$, the sequence is:
$$
2, 6, 18, 54, \dots
$$

---

## Fibonacci Sequence

### Definition:
The **Fibonacci sequence** is a famous recursive sequence where each term is the sum of the two preceding terms. The sequence is defined by the recurrence relation:
$$
F_n = F_{n-1} + F_{n-2}, \quad F_1 = 1, \quad F_2 = 1
$$
The first few terms of the Fibonacci sequence are:
$$
1, 1, 2, 3, 5, 8, 13, 21, 34, \dots
$$

### Properties of the Fibonacci Sequence:
- The Fibonacci sequence grows exponentially as $n$ increases.
- The ratio of consecutive Fibonacci numbers approaches the **golden ratio**:
$$
\lim_{n \to \infty} \frac{F_{n+1}}{F_n} = \frac{1 + \sqrt{5}}{2} \approx 1.618
$$

