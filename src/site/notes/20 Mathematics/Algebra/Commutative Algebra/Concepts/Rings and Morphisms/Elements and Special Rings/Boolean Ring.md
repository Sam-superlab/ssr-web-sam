---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Boolean Ring/","title":"Boolean Ring","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"],"dg-note-properties":{"title":"Boolean Ring","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"]}}
---


# Boolean Ring

A **Boolean ring** is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ in which every element is [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Idempotent\|Idempotent]]:

$$
x^2=x\qquad(x\in A).
$$

## Immediate consequences

Every Boolean ring has characteristic $2$. Applying idempotence to $x+x$ gives

$$
(2x)^2=2x.
$$

Using $x^2=x$, the left side is $4x$, so $2x=0$.

Every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|Prime Ideal]] is [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Maximal Ideal\|maximal]]. If $\mathfrak p$ is prime, $A/\mathfrak p$ is a Boolean [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]]. For any nonzero class $x$,

$$
x(x-1)=0
$$

forces $x=1$. Thus the quotient is the two-element field $\mathbb F_2$.

Every finitely generated ideal is principal. For example,

$$
(a,b)=(a+b+ab)
$$

in characteristic $2$.

## Examples

- The power set $\mathcal P(S)$ becomes a Boolean ring with symmetric difference as addition and intersection as multiplication.
- $\mathbb F_2^n$ is Boolean.
- $\mathbb Z/4\mathbb Z$ is not Boolean because $2^2\neq2$.

## Topology and lattices

The [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Core/Prime Spectrum\|Prime Spectrum]] of a Boolean ring is compact Hausdorff, and every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Core/Basic Open Set\|Basic Open Set]] is also closed. Exercises 24-25 identify Boolean rings with Boolean lattices and lead to Stone's representation theorem.

## Source

- 01_08_exercises.pdf, printed pp. 11 and 14; Exercises 11 and 23-25.

