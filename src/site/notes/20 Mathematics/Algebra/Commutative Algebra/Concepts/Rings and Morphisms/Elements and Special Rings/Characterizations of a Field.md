---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Characterizations of a Field/","title":"Characterizations of a Field","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"],"dg-note-properties":{"title":"Characterizations of a Field","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"]}}
---


# Characterizations of a Field

For a nonzero [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$, the following are equivalent:

1. $A$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Field\|Field]].
2. The only [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|ideals]] of $A$ are $(0)$ and $(1)$.
3. Every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring Homomorphism\|Ring Homomorphism]] from $A$ to a nonzero ring is injective.

## Proof

If $A$ is a field and $\mathfrak a\neq(0)$, choose $0\neq x\in\mathfrak a$. Since $x$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Unit\|Unit]], $1=x^{-1}x\in\mathfrak a$, so $\mathfrak a=A$.

Assume only $(0)$ and $(1)$ are ideals. For $f:A\to B$ with $B\neq0$, the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Kernel of a Ring Homomorphism\|kernel]] is an ideal. It cannot be $(1)$ because $f(1)=1_B\neq0$, so it is $(0)$ and $f$ is injective.

Finally, assume every map to a nonzero ring is injective. If $x$ is not a unit, then $(x)\neq(1)$ and $A/(x)$ is nonzero. The [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Canonical Projection\|Canonical Projection]] $A\to A/(x)$ must be injective, so $(x)=(0)$ and $x=0$. Thus every nonzero $x$ is a unit.

## Use

Combined with the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Correspondence Theorem for Ideals\|Correspondence Theorem for Ideals]], this proves

$$
\mathfrak m\text{ maximal}\iff A/\mathfrak m\text{ is a field}.
$$

## Source

- 01_03_zero_divisors_nilpotent_units.pdf, printed p. 3; Proposition 1.2.

