---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring Homomorphism/","dg-note-properties":{}}
---


# Ring Homomorphism

A **ring homomorphism** $f:A\to B$ is a map between [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring\|rings]] satisfying

$$
f(x+y)=f(x)+f(y),\qquad
f(xy)=f(x)f(y),\qquad
f(1_A)=1_B.
$$

The last condition is part of the definition here. It rules out maps such as the zero map $A\to B$ when $B$ is nonzero.

## Automatic properties

The additive-group law implies

$$
f(0)=0,\qquad f(-x)=-f(x),\qquad f(x-y)=f(x)-f(y).
$$

The composite of homomorphisms is a homomorphism. The identity map is one as well.

## Examples

- The [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Canonical Projection\|Canonical Projection]] $A\to A/\mathfrak a$ is surjective.
- Evaluation $k[x]\to k$, $p(x)\mapsto p(a)$, has [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Kernel of a Ring Homomorphism\|kernel]] $(x-a)$.
- The inclusion $\mathbb Z\hookrightarrow\mathbb Q$ is injective.
- The map $\mathbb Z\to\mathbb Z/n\mathbb Z$ sends an integer to its residue class.

Every homomorphism produces an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Image of a Ring Homomorphism\|image]] and a kernel, related by the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/First Isomorphism Theorem for Rings\|First Isomorphism Theorem for Rings]]. Ideals can also be transported by [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/07 Extension and Contraction/Extension of an Ideal\|extension]] and [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/07 Extension and Contraction/Contraction of an Ideal\|contraction]].

## Source

- 01_02_ideals_quotient_rings.pdf, printed p. 2 (definition and composition).
