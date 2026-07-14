---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Comaximal Ideal/","title":"Comaximal Ideal","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Comaximal Ideal","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Comaximal Ideal

Two [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|ideals]] $\mathfrak a,\mathfrak b$ in a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ are **comaximal** or **coprime** if

$$
\mathfrak a+\mathfrak b=A.
$$

Equivalently, there exist $a\in\mathfrak a$ and $b\in\mathfrak b$ such that

$$
a+b=1.
$$

## Product equals intersection

If $\mathfrak a+\mathfrak b=A$, then

$$
\mathfrak a\cap\mathfrak b=\mathfrak a\mathfrak b.
$$

Indeed, for $x\in\mathfrak a\cap\mathfrak b$ and $1=a+b$ as above,

$$
x=xa+xb.
$$

Here $xa\in\mathfrak b\mathfrak a$ because $x\in\mathfrak b$, and $xb\in\mathfrak a\mathfrak b$ because $x\in\mathfrak a$.

## Examples

- $(m)$ and $(n)$ in $\mathbb Z$ are comaximal exactly when $\gcd(m,n)=1$.
- Distinct [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Maximal Ideal\|maximal ideals]] are comaximal.
- $(x)$ and $(1-x)$ are comaximal in $k[x]$.

Pairwise comaximal ideals satisfy the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Chinese Remainder Theorem\|Chinese Remainder Theorem]]. Proposition 1.16 also says that if $\sqrt{\mathfrak a}$ and $\sqrt{\mathfrak b}$ are comaximal, then $\mathfrak a$ and $\mathfrak b$ already are.

## Source

- 01_06_operations_on_ideals.pdf, printed pp. 6-7 (definition and product-intersection equality); Proposition 1.16 on printed p. 9.

