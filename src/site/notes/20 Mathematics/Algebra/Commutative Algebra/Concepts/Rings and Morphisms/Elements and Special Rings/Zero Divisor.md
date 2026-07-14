---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Zero Divisor/","title":"Zero Divisor","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"],"dg-note-properties":{"title":"Zero Divisor","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"]}}
---


# Zero Divisor

An element $x$ of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ is a **nonzero zero divisor** if $x\neq0$ and there exists a nonzero $y\in A$ such that

$$
xy=0.
$$

Terminology varies. Many authors reserve “zero divisor” for such a nonzero $x$; Atiyah and Macdonald allow $x=0$ whenever it annihilates a nonzero element. Statements in this knowledge base say **nonzero zero divisor** when the distinction matters.

## Examples

- In $\mathbb Z/6\mathbb Z$, the classes of $2$ and $3$ are nonzero zero divisors.
- In $k[x,y]/(xy)$, the nonzero classes of $x$ and $y$ annihilate one another.
- In $\mathbb Z$, there are no nonzero zero divisors.

## Relations

Every nonzero [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Nilpotent Element\|Nilpotent Element]] is a nonzero zero divisor: if $x^n=0$ with $n$ minimal and $x\neq0$, then $x^{n-1}\neq0$ and $x\cdot x^{n-1}=0$.

A [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Unit\|Unit]] cannot be a zero divisor in a nonzero ring. If $xy=0$ and $x$ is invertible, multiplying by $x^{-1}$ gives $y=0$.

A nonzero commutative ring with no nonzero zero divisors is an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]]. The set of zero divisors need not be an ideal; in Noetherian settings it is controlled by [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Primary Decomposition and Associated Primes/Associated Primes and Components/Associated Prime\|associated primes]].

## Source

- 01_03_zero_divisors_nilpotent_units.pdf, printed p. 2 (definition and relation to domains).
