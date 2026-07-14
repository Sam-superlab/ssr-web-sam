---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Zero Ideal/","title":"Zero Ideal","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Zero Ideal","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Zero Ideal

The **zero ideal** of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ is

$$
(0)=\{0\}.
$$

It is commonly written simply as $0$ when the ambient ring is clear. The quotient $A/(0)$ is canonically isomorphic to $A$.

## Prime test

The zero ideal is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|Prime Ideal]] exactly when $A$ is an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]]:

$$
(0)\text{ prime}
\iff
ab=0\Longrightarrow a=0\text{ or }b=0.
$$

It is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Maximal Ideal\|Maximal Ideal]] exactly when $A$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Field\|Field]], provided $A\neq0$.

## Radical

The [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Radical of an Ideal\|Radical of an Ideal]] of $(0)$ is

$$
\sqrt{(0)}=\{x\in A:x^n=0\text{ for some }n>0\},
$$

which is the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Nilradical\|Nilradical]]. Hence the zero ideal is radical exactly when $A$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Reduced Ring\|Reduced Ring]].

## Caution

In the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Zero Ring\|Zero Ring]], $(0)=(1)=A$ is not proper. Therefore it is neither prime nor maximal under the standard definitions.

## Source

- 01_03_zero_divisors_nilpotent_units.pdf, printed p. 3 (notation for the zero ideal and its prime-ideal test).

