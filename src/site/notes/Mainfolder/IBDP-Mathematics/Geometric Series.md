---
{"dg-publish":true,"permalink":"/Mainfolder/IBDP-Mathematics/Geometric Series/"}
---

- [[Mainfolder/IBDP-Mathematics/Geometric Series#Formula for the Sum of a Geometric Series\|Formula for the Sum of a Geometric Series]]
	- [[Mainfolder/IBDP-Mathematics/Geometric Series#Formula for the Sum of a Geometric Series\|Formula for the Sum of the First $n$ Terms:]]
	- [[Mainfolder/IBDP-Mathematics/Geometric Series#Formula for the Sum of a Geometric Series\|Example:]]
- [[Mainfolder/IBDP-Mathematics/Geometric Series#Convergence of Geometric Series\|Convergence of Geometric Series]]
	- [[Mainfolder/IBDP-Mathematics/Geometric Series#Convergence of Geometric Series\|Infinite Geometric Series:]]
	- [[Mainfolder/IBDP-Mathematics/Geometric Series#Convergence of Geometric Series\|Example:]]
	- [[Mainfolder/IBDP-Mathematics/Geometric Series#Convergence of Geometric Series\|Divergence of Geometric Series:]]
	- [[Mainfolder/IBDP-Mathematics/Geometric Series#Convergence of Geometric Series\|Example of Divergence:]]
- [[Mainfolder/IBDP-Mathematics/Geometric Series#Applications of Geometric Series\|Applications of Geometric Series]]
	- [[Mainfolder/IBDP-Mathematics/Geometric Series#Applications of Geometric Series\|1. **Finance**: Calculating Compound Interest]]
		- [[Mainfolder/IBDP-Mathematics/Geometric Series#1. **Finance**: Calculating Compound Interest\|Example:]]
	- [[Mainfolder/IBDP-Mathematics/Geometric Series#Applications of Geometric Series\|2. **Physics**: Motion and Damping]]
		- [[Mainfolder/IBDP-Mathematics/Geometric Series#2. **Physics**: Motion and Damping\|Example:]]
	- [[Mainfolder/IBDP-Mathematics/Geometric Series#Applications of Geometric Series\|3. **Computer Science**: Algorithm Analysis]]
		- [[Mainfolder/IBDP-Mathematics/Geometric Series#3. **Computer Science**: Algorithm Analysis\|Example:]]
	- [[Mainfolder/IBDP-Mathematics/Geometric Series#Applications of Geometric Series\|4. **Signal Processing**: Fourier Series]]

## Formula for the Sum of a Geometric Series

A **geometric series** is a series where each term is obtained by multiplying the previous term by a constant ratio $r$. The general form of a geometric series is:
$$
S = a + ar + ar^2 + ar^3 + \dots
$$
Where:
- $a$ is the first term.
- $r$ is the common ratio (the factor by which each term is multiplied to get the next term).

### Formula for the Sum of the First $n$ Terms:
The sum of the first $n$ terms of a geometric series is given by:
$$
S_n = a \cdot \frac{1 - r^n}{1 - r}, \quad r \neq 1
$$
Where:
- $S_n$ is the sum of the first $n$ terms.
- $a$ is the first term.
- $r$ is the common ratio.
- $n$ is the number of terms.

### Example:
Find the sum of the first 5 terms of the geometric series where $a = 2$ and $r = 3$:
$$
S_5 = 2 \cdot \frac{1 - 3^5}{1 - 3} = 2 \cdot \frac{1 - 243}{1 - 3} = 2 \cdot \frac{-242}{-2} = 242
$$

---

## Convergence of Geometric Series

### Infinite Geometric Series:
An **infinite geometric series** is one where the number of terms approaches infinity. The sum of an infinite geometric series is given by the limit of the partial sums as $n \to \infty$.

If $|r| < 1$, the infinite geometric series converges, and the sum is:
$$
S = \frac{a}{1 - r}, \quad |r| < 1
$$
If $|r| \geq 1$, the series diverges.

### Example:
Find the sum of the infinite geometric series $S = 3 + 3 \cdot \frac{1}{2} + 3 \cdot \frac{1}{2}^2 + 3 \cdot \frac{1}{2}^3 + \dots$
- Here, $a = 3$ and $r = \frac{1}{2}$.
- Since $|r| = \frac{1}{2} < 1$, the series converges.
- The sum is:
$$
S = \frac{3}{1 - \frac{1}{2}} = \frac{3}{\frac{1}{2}} = 6
$$

### Divergence of Geometric Series:
If $|r| \geq 1$, the geometric series **diverges**. This means that the sum grows without bound as the number of terms increases, or the series does not approach a finite value.

### Example of Divergence:
The geometric series $S = 1 + 2 + 4 + 8 + \dots$ with $a = 1$ and $r = 2$ diverges because $|r| = 2 \geq 1$.

---

## Applications of Geometric Series

### 1. **Finance**: Calculating Compound Interest
Geometric series are used in finance to calculate the future value of investments with compound interest.

#### Example:
Consider an investment with an initial amount $P$, annual interest rate $r$, compounded annually for $n$ years. The total value $A$ of the investment after $n$ years is:
$$
A = P(1 + r)^n
$$
This formula comes from summing the powers of $(1 + r)$ over time, which is a geometric series.

### 2. **Physics**: Motion and Damping
Geometric series arise in physics when studying systems with exponential decay or damping, where successive displacements or amplitudes form a geometric sequence.

#### Example:
A ball dropped from a height that bounces back to half its height each time forms a geometric series. The total distance the ball travels before coming to rest is:
$$
S = h + 2 \left(\frac{h}{2} + \frac{h}{4} + \frac{h}{8} + \dots \right)
$$
Where $h$ is the initial height.

### 3. **Computer Science**: Algorithm Analysis
Geometric series are used in computer science to analyze the time complexity of recursive algorithms, particularly those that involve dividing a problem into smaller subproblems.

#### Example:
In the **merge sort** algorithm, each recursive division step splits the input array in half, forming a geometric series in terms of time complexity.

### 4. **Signal Processing**: Fourier Series
Geometric series are applied in signal processing to represent periodic functions as sums of sines and cosines, enabling frequency analysis in signals.

