---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Direct Constructions and Limits/Direct Product/","title":"Direct Product","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"],"dg-note-properties":{"title":"Direct Product","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"]}}
---


# Direct Product

For $A$-modules $(M_i)_{i\in I}$, the **direct product**

$$\prod_{i\in I}M_i$$

contains every tuple $(m_i)$ with $m_i\in M_i$, with no finite-support condition. Addition and scalar multiplication are coordinatewise.

If $I$ is finite, the direct product equals the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Direct Constructions and Limits/Direct Sum\|Direct Sum]]. If $I$ is infinite, the sum is generally a proper submodule of the product.

## Example

For $M_i=A$, the tuple $(1,1,1,\ldots)$ lies in $\prod_{i\ge0}A$ but not in $\bigoplus_{i\ge0}A$ when $A\neq0$.

## Intuition

A direct sum is assembled from finitely many active coordinates at a time. A direct product stores a simultaneous choice in every coordinate. This difference matters only for infinite families.

## Source

- `02_04_direct_sum_and_product.pdf`, printed p. 20.
