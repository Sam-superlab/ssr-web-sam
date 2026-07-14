---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Radical of an Ideal/","title":"Radical of an Ideal","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Radical of an Ideal","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Radical of an Ideal

For an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] $\mathfrak a$ of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$, its **radical** is

$$
\sqrt{\mathfrak a}
=
\{x\in A:x^n\in\mathfrak a\text{ for some }n>0\}.
$$

It is an ideal because it is the inverse image of the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Nilradical\|Nilradical]] of $A/\mathfrak a$ under the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Canonical Projection\|Canonical Projection]].

An ideal is **radical** if $\sqrt{\mathfrak a}=\mathfrak a$.

## Basic identities

$$
\mathfrak a\subseteq\sqrt{\mathfrak a},
\qquad
\sqrt{\sqrt{\mathfrak a}}=\sqrt{\mathfrak a},
$$

$$
\sqrt{\mathfrak a\mathfrak b}
=
\sqrt{\mathfrak a\cap\mathfrak b}
=
\sqrt{\mathfrak a}\cap\sqrt{\mathfrak b},
$$

$$
\sqrt{\mathfrak a}=(1)\iff\mathfrak a=(1).
$$

Every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|Prime Ideal]] is radical. Also $\sqrt{\mathfrak p^n}=\mathfrak p$ for prime $\mathfrak p$.

## Examples

- In $\mathbb Z$, if $m$ has distinct prime divisors $p_1,\ldots,p_r$, then

$$
\sqrt{(m)}=(p_1\cdots p_r).
$$

- $\sqrt{(x^2,y^3)}=(x,y)$ in $k[x,y]$.
- $\sqrt{(0)}$ is the nilradical.

The structural description is [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Radical as an Intersection of Prime Ideals\|Radical as an Intersection of Prime Ideals]]:

$$
\sqrt{\mathfrak a}
=
\bigcap_{\mathfrak p\supseteq\mathfrak a}\mathfrak p.
$$

## Source

- 01_06_operations_on_ideals.pdf, printed pp. 8-9; Exercise 1.13 and Proposition 1.14.

