---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/08 Exercises and Further Directions/Regular Map/","dg-note-properties":{}}
---


# Regular Map

Let $X\subseteq k^n$ and $Y\subseteq k^m$ be [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/08 Exercises and Further Directions/Affine Algebraic Variety\|affine algebraic varieties]]. A map

$$
\varphi:X\to Y
$$

is **regular** if its coordinate functions are polynomial functions on $X$. Equivalently, it is the restriction to $X$ of a polynomial map $k^n\to k^m$ whose image lies in $Y$.

## Pullback of functions

Every regular map induces a $k$-algebra homomorphism between [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/08 Exercises and Further Directions/Coordinate Ring\|coordinate rings]] in the opposite direction:

$$
\varphi^*:P(Y)\to P(X),
\qquad
g\longmapsto g\circ\varphi.
$$

Composition reverses:

$$
(\psi\circ\varphi)^*=\varphi^*\circ\psi^*.
$$

## Algebra-geometry correspondence

Exercise 28 proves a bijection

$$
\{\text{regular maps }X\to Y\}
\longleftrightarrow
\{k\text{-algebra homomorphisms }P(Y)\to P(X)\}.
$$

Given a homomorphism $P(Y)\to P(X)$, the images of the coordinate functions on $Y$ provide the coordinate polynomials of the corresponding map $X\to Y$.

## Example

The parametrization

$$
\mathbb A^1\to V(y-x^2),
\qquad
t\mapsto(t,t^2)
$$

is regular. On coordinate rings it corresponds to

$$
k[x,y]/(y-x^2)\to k[t],
\qquad
x\mapsto t,\ y\mapsto t^2.
$$

## Source

- 01_08_exercises.pdf, printed p. 16; Exercise 28.

