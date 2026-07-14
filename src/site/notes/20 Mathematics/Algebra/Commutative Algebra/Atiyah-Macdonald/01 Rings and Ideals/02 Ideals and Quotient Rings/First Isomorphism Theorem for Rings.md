---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/First Isomorphism Theorem for Rings/","dg-note-properties":{}}
---


# First Isomorphism Theorem for Rings

Let $f:A\to B$ be a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring Homomorphism\|Ring Homomorphism]]. Then $f$ induces a canonical [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring Isomorphism\|Ring Isomorphism]]

$$
\bar f:A/\ker f\longrightarrow\operatorname{im}f,
\qquad
a+\ker f\longmapsto f(a).
$$

## Proof

The formula is well defined: if $a+\ker f=a'+\ker f$, then $a-a'\in\ker f$, so $f(a)=f(a')$. It is a homomorphism because $f$ preserves the ring operations. It is surjective by the definition of [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Image of a Ring Homomorphism\|image]], and its kernel is zero. Hence it is injective.

## Meaning

Every ring homomorphism factors as

$$
A\twoheadrightarrow A/\ker f
\xrightarrow{\ \cong\ }\operatorname{im}f
\hookrightarrow B.
$$

The theorem separates the two possible failures of a map to be an isomorphism: it may kill information through its [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Kernel of a Ring Homomorphism\|kernel]], and its image may be smaller than the codomain.

## Example

For evaluation at $a$,

$$
k[x]/(x-a)\cong k.
$$

For reduction modulo $n$,

$$
\mathbb Z/(n)\cong\mathbb Z/n\mathbb Z.
$$

## Source

- 01_02_ideals_quotient_rings.pdf, printed p. 2 (induced isomorphism $A/\ker f\cong f(A)$).
