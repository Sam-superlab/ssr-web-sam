---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Change of Scalars/Restriction of Scalars/","title":"Restriction of Scalars","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"],"dg-note-properties":{"title":"Restriction of Scalars","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"]}}
---


# Restriction of Scalars

Given a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring Homomorphism\|Ring Homomorphism]] $f:A\to B$ and a $B$-module $N$, **restriction of scalars** makes $N$ an $A$-module by

$$a\cdot n=f(a)n.$$

The underlying abelian group and elements do not change. Only the permitted scalar action is viewed through $f$.

## Examples

- A complex vector space becomes a real vector space along $\mathbb R\hookrightarrow\mathbb C$.
- A module over $A/I$ becomes an $A$-module on which $I$ acts by zero.
- The ring $B$ itself becomes an $A$-module along $f$; this is the module structure behind an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Algebras over Rings/Core/Algebra over a Ring\|Algebra over a Ring]].

Proposition 2.16: if $B$ is finitely generated as an $A$-module and $N$ is finitely generated as a $B$-module, then the restricted $A$-module $N$ is finitely generated.

The opposite-direction construction is [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Change of Scalars/Extension of Scalars\|Extension of Scalars]].

## Source

- `02_08_restriction_and_extension_of_scalars.pdf`, printed pp. 27-28; Proposition 2.16.
