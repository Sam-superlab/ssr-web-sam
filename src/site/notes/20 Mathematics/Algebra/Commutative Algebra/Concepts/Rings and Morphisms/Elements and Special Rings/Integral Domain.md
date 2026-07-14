---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain/","title":"Integral Domain","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"],"dg-note-properties":{"title":"Integral Domain","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"]}}
---


# Integral Domain

An **integral domain** is a nonzero [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ with no nonzero [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Zero Divisor\|zero divisors]]. Thus

$$
ab=0\quad\Longrightarrow\quad a=0\text{ or }b=0.
$$

## Equivalent cancellation law

In a commutative ring with $1\neq0$, the domain condition is equivalent to cancellation:

$$
a\neq0,\ ab=ac\quad\Longrightarrow\quad b=c.
$$

Indeed, $ab=ac$ gives $a(b-c)=0$.

## Examples and nonexamples

- $\mathbb Z$ is an integral domain.
- Every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Field\|Field]] is an integral domain.
- If $k$ is a field, $k[x_1,\ldots,x_n]$ is an integral domain.
- $\mathbb Z/6\mathbb Z$ is not a domain because $2\cdot3=0$.
- The [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Zero Ring\|Zero Ring]] is excluded by the requirement $1\neq0$.

## Ideal test

An [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] $\mathfrak p$ is [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|prime]] exactly when

$$
A/\mathfrak p
$$

is an integral domain. In particular, the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Zero Ideal\|Zero Ideal]] is prime exactly when $A$ itself is an integral domain.

## Source

- 01_03_zero_divisors_nilpotent_units.pdf, printed p. 2 (definition and examples); quotient characterization appears on printed p. 3.

