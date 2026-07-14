---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Direct Product of Rings/","title":"Direct Product of Rings","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"],"dg-note-properties":{"title":"Direct Product of Rings","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"]}}
---


# Direct Product of Rings

For [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|rings]] $A_1,\ldots,A_n$, their **direct product** is

$$
\prod_{i=1}^n A_i
=
\{(a_1,\ldots,a_n):a_i\in A_i\},
$$

with componentwise addition and multiplication. Its identity is $(1,\ldots,1)$.

Each projection

$$
\pi_i:\prod_jA_j\to A_i,\qquad
(a_1,\ldots,a_n)\mapsto a_i
$$

is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring Homomorphism\|Ring Homomorphism]].

## Examples

- $\mathbb Z/6\mathbb Z\cong\mathbb Z/2\mathbb Z\times\mathbb Z/3\mathbb Z$ by the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Chinese Remainder Theorem\|Chinese Remainder Theorem]].
- A product of two nonzero rings has nontrivial [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Idempotent\|idempotents]] $(1,0)$ and $(0,1)$.
- A product of two nonzero rings is never an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]], since $(1,0)(0,1)=0$.

## Ideals

Every ideal of a finite product $A_1\times\cdots\times A_n$ has the form

$$
\mathfrak a_1\times\cdots\times\mathfrak a_n
$$

with $\mathfrak a_i\triangleleft A_i$. The prime spectrum is consequently the disjoint union of the spectra of the factors, a theme developed in Exercise 22.

## Sources

- 01_06_operations_on_ideals.pdf, printed p. 7 (definition and projection homomorphisms).
- 01_08_exercises.pdf, printed pp. 13-14; Exercise 22 (ideals, spectra, and product decompositions).
