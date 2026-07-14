---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Annihilator in a Ring/","title":"Annihilator in a Ring","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Annihilator in a Ring","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Annihilator in a Ring

For an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] $\mathfrak b$ of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$, its **annihilator** is

$$
\operatorname{Ann}(\mathfrak b)
=(0:\mathfrak b)
=
\{x\in A:x\mathfrak b=0\}.
$$

For an element $b\in A$, one writes

$$
\operatorname{Ann}(b)
=
\{x\in A:xb=0\}
=
(0:b).
$$

Both are ideals.

## Examples

- In an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]], $\operatorname{Ann}(b)=(0)$ for every nonzero $b$.
- In $\mathbb Z/12\mathbb Z$, $\operatorname{Ann}(4)=(3)$.
- In $k[x,y]/(xy)$, $y\in\operatorname{Ann}(x)$ and $x\in\operatorname{Ann}(y)$.

## Zero divisors

The set of [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Zero Divisor\|zero divisors]] is

$$
\bigcup_{0\neq x\in A}\operatorname{Ann}(x).
$$

This union is not generally an ideal. Proposition 1.15 refines the description using radicals:

$$
D
=
\bigcup_{0\neq x\in A}\sqrt{\operatorname{Ann}(x)}.
$$

The annihilator is a special case of the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal Quotient\|Ideal Quotient]] and will later generalize naturally to modules.

## Source

- 01_06_operations_on_ideals.pdf, printed pp. 8-9 (annihilator definition and Proposition 1.15).

