---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Multilinear Map/","title":"Multilinear Map","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"],"dg-note-properties":{"title":"Multilinear Map","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"]}}
---


# Multilinear Map

A map $f:M_1\times\cdots\times M_r\to P$ is **multilinear** if it is $A$-linear in each variable separately.

Proposition 2.12* generalizes the tensor universal property: there is a module

$$M_1\otimes_A\cdots\otimes_A M_r$$

such that multilinear maps from the Cartesian product to $P$ correspond uniquely to linear maps from this iterated tensor product to $P$.

The [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Standard Isomorphisms for Tensor Products\|associativity isomorphism]] means parentheses may usually be suppressed, though this is a canonical isomorphism rather than literal equality.

## Example

The determinant is an alternating multilinear map of the columns of a square matrix. Exterior powers are built by imposing alternating relations in addition to multilinearity.

## Source

- `02_07_tensor_product_of_modules.pdf`, printed p. 26; Proposition 2.12*.
