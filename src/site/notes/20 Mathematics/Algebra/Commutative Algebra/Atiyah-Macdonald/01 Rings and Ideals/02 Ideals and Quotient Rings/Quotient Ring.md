---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Quotient Ring/","dg-note-properties":{}}
---


# Quotient Ring

Let $\mathfrak a$ be an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Ideal\|Ideal]] of a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring\|Ring]] $A$. The **quotient ring** $A/\mathfrak a$ consists of additive cosets

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

Passing from $A$ to $A/\mathfrak a$ declares every element of $\mathfrak a$ equal to zero. More generally, two elements have the same residue class exactly when they are [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Congruence Modulo an Ideal\|congruent modulo $\mathfrak a$]].

## Examples

- $\mathbb Z/(n)$ is the ring of residue classes modulo $n$.
- $k[x]/(x-a)\cong k$ by evaluation at $a$.
- $k[x]/(x^2)$ has a nonzero [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/03 Zero Divisors Nilpotents and Units/Nilpotent Element\|Nilpotent Element]], namely the class of $x$.
- $A/A$ is the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Zero Ring\|Zero Ring]], while $A/(0)\cong A$.

## Quotient tests

Quotients characterize distinguished ideals:

$$
\mathfrak p\text{ prime}\iff A/\mathfrak p\text{ is an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/03 Zero Divisors Nilpotents and Units/Integral Domain\|Integral Domain]]},
$$

$$
\mathfrak m\text{ maximal}\iff A/\mathfrak m\text{ is a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/03 Zero Divisors Nilpotents and Units/Field\|Field]]}.
$$

Ideals of the quotient are controlled by the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Correspondence Theorem for Ideals\|Correspondence Theorem for Ideals]].

## Source

- 01_02_ideals_quotient_rings.pdf, printed p. 2 (quotient or residue-class ring).

