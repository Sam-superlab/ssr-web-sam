---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Quotient Ring/","title":"Quotient Ring","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Quotient Ring","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Quotient Ring

Let $\mathfrak a$ be an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$. The **quotient ring** $A/\mathfrak a$ consists of additive cosets

$$
x+\mathfrak a=\{x+a:a\in\mathfrak a\},
$$

with operations

$$
(x+\mathfrak a)+(y+\mathfrak a)=(x+y)+\mathfrak a,
$$

$$
(x+\mathfrak a)(y+\mathfrak a)=xy+\mathfrak a.
$$

Ideal absorption makes the product independent of the chosen representatives.

## Interpretation

Passing from $A$ to $A/\mathfrak a$ declares every element of $\mathfrak a$ equal to zero. More generally, two elements have the same residue class exactly when they are [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Congruence Modulo an Ideal\|congruent modulo $\mathfrak a$]].

## Examples

- $\mathbb Z/(n)$ is the ring of residue classes modulo $n$.
- $k[x]/(x-a)\cong k$ by evaluation at $a$.
- $k[x]/(x^2)$ has a nonzero [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Nilpotent Element\|Nilpotent Element]], namely the class of $x$.
- $A/A$ is the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Zero Ring\|Zero Ring]], while $A/(0)\cong A$.

## Quotient tests

Quotients characterize distinguished ideals:

$$
\mathfrak p\text{ prime}\iff A/\mathfrak p\text{ is an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]]},
$$

$$
\mathfrak m\text{ maximal}\iff A/\mathfrak m\text{ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Field\|Field]]}.
$$

Ideals of the quotient are controlled by the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Correspondence Theorem for Ideals\|Correspondence Theorem for Ideals]].

## Source

- 01_02_ideals_quotient_rings.pdf, printed p. 2 (quotient or residue-class ring).

