---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Standard Isomorphisms for Tensor Products/","title":"Standard Isomorphisms for Tensor Products","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"],"dg-note-properties":{"title":"Standard Isomorphisms for Tensor Products","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"],"aliases":["Canonical Tensor Isomorphism"]}}
---


# Standard Isomorphisms for Tensor Products

For $A$-modules $M,N,P$, there are natural isomorphisms

$$
M\otimes_A N\cong N\otimes_A M,
$$

$$
(M\otimes_A N)\otimes_A P\cong M\otimes_A(N\otimes_A P),
$$

$$
(M\oplus N)\otimes_A P\cong(M\otimes_A P)\oplus(N\otimes_A P),
$$

$$
A\otimes_A M\cong M.
$$

They act on pure tensors in the expected ways: swap the factors, remove parentheses, distribute coordinates, or multiply $a\otimes m\mapsto am$.

## Proof pattern

Writing a plausible formula is not enough, because tensors are equivalence classes. Use the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Tensor Product Universal Property\|Tensor Product Universal Property]] to build the map from a bilinear or multilinear formula, build an inverse the same way, then check both composites on [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Pure Tensor\|pure tensors]], which generate the tensor product.

“Canonical” means that the maps require no choices and are natural with respect to module homomorphisms.

## Source

- `02_07_tensor_product_of_modules.pdf`, printed pp. 26–27; Proposition 2.14.
