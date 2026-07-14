---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Direct Constructions and Limits/Direct Sum Decomposition of a Module/","title":"Direct Sum Decomposition of a Module","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"],"dg-note-properties":{"title":"Direct Sum Decomposition of a Module","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"],"aliases":["Module Decomposition"]}}
---


# Direct Sum Decomposition of a Module
A **module decomposition** expresses a module as an internal [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Direct Constructions and Limits/Direct Sum\|Direct Sum]] of submodules. For example,

$$M=M_1\oplus M_2$$

means $M=M_1+M_2$ and $M_1\cap M_2=0$, so every $m\in M$ has a unique form $m_1+m_2$.

For the regular module $A$, decompositions into ideals are controlled by [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Idempotent\|idempotents]]. If $1=e_1+\cdots+e_n$ with $e_i^2=e_i$ and $e_ie_j=0$ for $i\neq j$, then

$$A=Ae_1\oplus\cdots\oplus Ae_n.$$

Conversely, a finite direct-sum decomposition of $A$ into ideals produces such idempotents and therefore a product decomposition of the ring. Geometrically, nontrivial idempotents signal that the ring has disconnected pieces.

## Source

- `02_04_direct_sum_and_product.pdf`, printed p. 20.
