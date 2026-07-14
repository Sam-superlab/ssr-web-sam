---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Jacobson Radical/","title":"Jacobson Radical","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Jacobson Radical","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Jacobson Radical

The **Jacobson radical** of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ is the intersection of all its [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Maximal Ideal\|maximal ideals]]:

$$
J(A)=\bigcap_{\mathfrak m\in\operatorname{Max}A}\mathfrak m.
$$

An element lies in $J(A)$ exactly when it vanishes in every field quotient $A/\mathfrak m$.

## Relation to the nilradical

Every maximal ideal is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|Prime Ideal]], so

$$
\operatorname{Nil}(A)\subseteq J(A).
$$

Equality need not hold. For the local domain $k[x]_{(x)}$, the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Nilradical\|Nilradical]] is $(0)$ while the Jacobson radical is the nonzero ideal $(x)$.

## Examples

- If $K$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Field\|Field]], then $J(K)=(0)$.
- If $(A,\mathfrak m)$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Local Algebra/Core/Local Ring\|Local Ring]], then $J(A)=\mathfrak m$.
- $J(\mathbb Z)=(0)$ because the intersection of all ideals $(p)$ is zero.
- $J(\mathbb Z/12\mathbb Z)=(6)$, the intersection of its two maximal ideals $(2)$ and $(3)$.

## Intrinsic test

The [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Jacobson Radical Unit Test\|Jacobson Radical Unit Test]] removes explicit reference to maximal ideals:

$$
x\in J(A)
\iff
1-xy\text{ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Unit\|Unit]] for every }y\in A.
$$

This criterion is often more practical in calculations.

## Source

- 01_05_nilradical_jacobson_radical.pdf, printed pp. 5-6; definition and Proposition 1.9.

