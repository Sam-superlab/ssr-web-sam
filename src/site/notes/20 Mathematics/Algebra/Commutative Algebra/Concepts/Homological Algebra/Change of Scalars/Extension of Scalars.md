---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Change of Scalars/Extension of Scalars/","title":"Extension of Scalars","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"],"dg-note-properties":{"title":"Extension of Scalars","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"]}}
---


# Extension of Scalars

Given a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring Homomorphism\|Ring Homomorphism]] $f:A\to B$ and an $A$-module $M$, the **extension of scalars from $A$ to $B$** is the $B$-module

$$B\otimes_A M,$$

with $B$-action $b(b'\otimes m)=bb'\otimes m$. The notation $M_B$ is sometimes used when the structure map $A\to B$ is understood, but $B\otimes_A M$ displays the change of rings explicitly.

The canonical map $M\to B\otimes_A M$ sends $m\mapsto1\otimes m$. It need not be injective or surjective in general.

## Examples

- $\mathbb C\otimes_{\mathbb R}V$ complexifies a real vector space.
- $(A/I)\otimes_A M\cong M/IM$.
- Localization is a scalar extension: $S^{-1}A\otimes_A M\cong S^{-1}M$.

Proposition 2.17: if $M$ is finitely generated over $A$, then $B\otimes_A M$ is finitely generated over $B$ by the tensors $1\otimes x_i$ from any generating set.

Extension of scalars is left adjoint to [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Change of Scalars/Restriction of Scalars\|Restriction of Scalars]], a close relative of the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Tensor-Hom Adjunction\|Tensor-Hom Adjunction]].

## Source

- `02_08_restriction_and_extension_of_scalars.pdf`, printed p. 28; Proposition 2.17.
