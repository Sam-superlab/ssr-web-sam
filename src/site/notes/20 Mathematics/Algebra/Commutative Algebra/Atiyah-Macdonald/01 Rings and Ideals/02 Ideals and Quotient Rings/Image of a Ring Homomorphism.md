---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Image of a Ring Homomorphism/","dg-note-properties":{}}
---


# Image of a Ring Homomorphism

For a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring Homomorphism\|Ring Homomorphism]] $f:A\to B$, the **image** is

$$
\operatorname{im}f=f(A)=\{f(a):a\in A\}.
$$

It is a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Subring\|Subring]] of $B$: it contains $1_B=f(1_A)$ and is closed under subtraction and multiplication.

The image need not be an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Ideal\|Ideal]] of $B$. For example, the image of $\mathbb Z\hookrightarrow\mathbb Q$ is $\mathbb Z$, which is not absorbed by multiplication by arbitrary rationals.

## Relation to the domain

The [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/First Isomorphism Theorem for Rings\|First Isomorphism Theorem for Rings]] gives

$$
A/\ker f\cong\operatorname{im}f.
$$

So the image is obtained from $A$ by identifying precisely those pairs whose difference lies in the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Kernel of a Ring Homomorphism\|kernel]].

## Examples

- Evaluation $k[x]\to k$ has image $k$.
- The map $\mathbb Z\to\mathbb Z/6\mathbb Z$ is surjective, so its image is the entire quotient.
- The map $\mathbb Z\to\mathbb Z$, $n\mapsto 2n$, is not a unital ring homomorphism: its apparent image $2\mathbb Z$ does not contain $1$.

## Source

- 01_02_ideals_quotient_rings.pdf, printed p. 2 (image as a subring).
