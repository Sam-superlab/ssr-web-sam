---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Tensor Product Universal Property/","title":"Tensor Product Universal Property","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"],"dg-note-properties":{"title":"Tensor Product Universal Property","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"]}}
---


# Tensor Product Universal Property

The tensor product comes with a canonical [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Bilinear Map\|Bilinear Map]]

$$\tau:M\times N\to M\otimes_A N,\qquad (x,y)\mapsto x\otimes y,$$

such that every bilinear $b:M\times N\to P$ factors uniquely through a linear map $\widetilde b:M\otimes_A N\to P$:

$$b=\widetilde b\circ\tau.$$

Equivalently,

$$\operatorname{Bilin}_A(M,N;P)\cong\operatorname{Hom}_A(M\otimes_A N,P)$$

naturally in $P$.

## Why it is the real definition

Any two modules with this property are uniquely isomorphic in a way compatible with their canonical bilinear maps. Therefore the construction by generators and relations is only one model; calculations should normally use the universal property.

To define a map out of a tensor product, define a bilinear map on pairs. To prove two maps out are equal, check them on all [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Pure Tensor\|pure tensors]].

## Source

- `02_07_tensor_product_of_modules.pdf`, printed pp. 24-25; Proposition 2.12.
