---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal Quotient/","title":"Ideal Quotient","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Ideal Quotient","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Ideal Quotient

For [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|ideals]] $\mathfrak a,\mathfrak b$ of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$, the **ideal quotient** is

$$
(\mathfrak a:\mathfrak b)
=
\{x\in A:x\mathfrak b\subseteq\mathfrak a\}.
$$

It is an ideal. If $\mathfrak b=(b)$ is principal, one writes $(\mathfrak a:b)$.

## Interpretation

The ideal quotient is the largest ideal $\mathfrak c$ satisfying

$$
\mathfrak c\mathfrak b\subseteq\mathfrak a.
$$

Thus it behaves like division of ideals without requiring an inverse.

## Basic identities

$$
\mathfrak a\subseteq(\mathfrak a:\mathfrak b),
\qquad
(\mathfrak a:\mathfrak b)\mathfrak b\subseteq\mathfrak a,
$$

$$
((\mathfrak a:\mathfrak b):\mathfrak c)
=
(\mathfrak a:\mathfrak b\mathfrak c),
$$

$$
\left(\bigcap_i\mathfrak a_i:\mathfrak b\right)
=
\bigcap_i(\mathfrak a_i:\mathfrak b).
$$

The special case $(0:\mathfrak b)$ is the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Annihilator in a Ring\|annihilator]] of $\mathfrak b$.

## Example

In $\mathbb Z$,

$$
((m):(n))
=
\left(\frac{m}{\gcd(m,n)}\right).
$$

For example, $((12):(8))=(3)$ because $8x$ is divisible by $12$ exactly when $x$ is divisible by $3$.

## Source

- 01_06_operations_on_ideals.pdf, printed p. 8; definition and Exercise 1.12.

