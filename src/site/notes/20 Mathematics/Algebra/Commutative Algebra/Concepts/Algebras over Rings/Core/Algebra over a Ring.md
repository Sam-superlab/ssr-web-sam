---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Algebras over Rings/Core/Algebra over a Ring/","title":"Algebra over a Ring","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/algebras-over-rings"],"dg-note-properties":{"title":"Algebra over a Ring","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/algebras-over-rings"]}}
---


# Algebra over a Ring

In commutative algebra, an **$A$-algebra** is a commutative [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $B$ together with a specified [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring Homomorphism\|Ring Homomorphism]]

$$f:A\to B.$$

This is the standing meaning in this knowledge base. In broader algebra, $B$ may be noncommutative and the structure map is then usually required to land in the center of $B$.

It becomes an $A$-module by $a\cdot b=f(a)b$. The module and ring structures satisfy

$$a(bb')=(ab)b'=b(ab').$$

## Examples

- $A[x_1,\ldots,x_n]$ is an $A$-algebra by including constants.
- Every quotient $A/I$ is an $A$-algebra via the quotient map.
- Every ring is a $\mathbb Z$-algebra through $n\mapsto n1$.
- If $K$ is a field and $B\neq0$, a $K$-algebra structure embeds $K$ as a specified subfield of $B$.

The structure map matters: the same underlying ring can carry different $A$-algebra structures. Maps respecting it are [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Algebras over Rings/Core/Algebra Homomorphism\|algebra homomorphisms]].

## Source

- `02_10_algebras.pdf`, printed pp. 29-30.
