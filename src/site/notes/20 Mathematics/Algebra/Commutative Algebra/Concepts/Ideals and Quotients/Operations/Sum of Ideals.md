---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Sum of Ideals/","title":"Sum of Ideals","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Sum of Ideals","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Sum of Ideals

For [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|ideals]] $\mathfrak a,\mathfrak b$ of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$, their **sum** is

$$
\mathfrak a+\mathfrak b
=
\{a+b:a\in\mathfrak a,\ b\in\mathfrak b\}.
$$

It is the smallest ideal containing both $\mathfrak a$ and $\mathfrak b$.

For an arbitrary family $\{\mathfrak a_i\}_{i\in I}$,

$$
\sum_{i\in I}\mathfrak a_i
$$

consists of finite sums $\sum_i a_i$ with $a_i\in\mathfrak a_i$ and all but finitely many $a_i$ equal to zero.

## Examples

- In $\mathbb Z$, $(m)+(n)=(\gcd(m,n))$.
- In $k[x,y]$, $(x)+(y)=(x,y)$.
- $\mathfrak a+(0)=\mathfrak a$ and $\mathfrak a+A=A$.

## Relations

Two ideals are [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Comaximal Ideal\|comaximal]] when their sum is $A$. Products distribute over sums:

$$
\mathfrak a(\mathfrak b+\mathfrak c)
=
\mathfrak a\mathfrak b+\mathfrak a\mathfrak c.
$$

If $\mathfrak b\subseteq\mathfrak a$, the modular law reads

$$
\mathfrak a\cap(\mathfrak b+\mathfrak c)
=
\mathfrak b+(\mathfrak a\cap\mathfrak c).
$$

## Source

- 01_06_operations_on_ideals.pdf, printed p. 6 (sum and arbitrary sum of ideals).

