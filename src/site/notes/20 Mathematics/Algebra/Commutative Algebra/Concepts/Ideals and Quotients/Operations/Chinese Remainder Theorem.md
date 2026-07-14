---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Chinese Remainder Theorem/","title":"Chinese Remainder Theorem","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Chinese Remainder Theorem","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Chinese Remainder Theorem

Let $\mathfrak a_1,\ldots,\mathfrak a_n$ be [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|ideals]] of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$. Define

$$
\varphi:A\to\prod_{i=1}^n A/\mathfrak a_i,
\qquad
x\mapsto(x+\mathfrak a_1,\ldots,x+\mathfrak a_n).
$$

Then:

1. $\ker\varphi=\bigcap_i\mathfrak a_i$.
2. $\varphi$ is surjective exactly when the $\mathfrak a_i$ are pairwise [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Comaximal Ideal\|comaximal]].
3. For pairwise comaximal ideals,

$$
\bigcap_i\mathfrak a_i=\prod_i\mathfrak a_i.
$$

Consequently,

$$
A\Big/\bigcap_i\mathfrak a_i
\cong
\prod_i A/\mathfrak a_i.
$$

## Construction of a solution

For each $i$, pairwise comaximality lets one find an element $e_i$ satisfying

$$
e_i\equiv1\pmod{\mathfrak a_i},
\qquad
e_i\equiv0\pmod{\mathfrak a_j}\quad(j\neq i).
$$

Given residues $r_i$, the element $\sum_i r_ie_i$ realizes them simultaneously.

## Example

Because $(3)+(5)=\mathbb Z$,

$$
\mathbb Z/15\mathbb Z
\cong
\mathbb Z/3\mathbb Z\times\mathbb Z/5\mathbb Z.
$$

The theorem fails without comaximality: the map $\mathbb Z\to\mathbb Z/2\times\mathbb Z/4$ is not surjective, since the two residues must agree modulo $2$.

## Source

- 01_06_operations_on_ideals.pdf, printed p. 7; Proposition 1.10.

