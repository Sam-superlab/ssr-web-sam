---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Tensor-Hom Adjunction/","title":"Tensor-Hom Adjunction","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"],"dg-note-properties":{"title":"Tensor-Hom Adjunction","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"]}}
---


# Tensor-Hom Adjunction

For $A$-modules $M,N,P$, there is a natural isomorphism

$$
\operatorname{Hom}_A(M\otimes_A N,P)
\cong
\operatorname{Hom}_A\bigl(M,\operatorname{Hom}_A(N,P)\bigr).
$$

A map $F:M\otimes_A N\to P$ corresponds to the map sending $x\in M$ to the homomorphism $y\mapsto F(x\otimes y)$. Conversely, a map $M\to\operatorname{Hom}_A(N,P)$ defines a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Bilinear Map\|Bilinear Map]] $(x,y)\mapsto\varphi(x)(y)$ and hence a map out of the tensor product.

## Meaning

A bilinear operation can be encoded in two equivalent ways: combine the inputs using a tensor product, or “curry” the operation into a family of linear maps.

In categorical language, $-\otimes_A N$ is left adjoint to $\operatorname{Hom}_A(N,-)$. Left adjoints preserve cokernels, which explains the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Right Exactness of Tensor Product\|Right Exactness of Tensor Product]]; right adjoints preserve kernels, matching [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Exact Sequences/Left Exactness of Hom\|Left Exactness of Hom]].

## Source

- `02_08_restriction_and_extension_of_scalars.pdf`, printed p. 28; canonical isomorphism (1) before Proposition 2.18.
