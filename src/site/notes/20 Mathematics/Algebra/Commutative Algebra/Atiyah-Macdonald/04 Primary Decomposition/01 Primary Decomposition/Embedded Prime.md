---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/04 Primary Decomposition/01 Primary Decomposition/Embedded Prime/","dg-note-properties":{}}
---


# Embedded Prime

An **embedded prime** of a decomposable ideal $\mathfrak a$ is an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/04 Primary Decomposition/01 Primary Decomposition/Associated Prime\|Associated Prime]] that is not minimal among the associated primes. It strictly contains an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/04 Primary Decomposition/01 Primary Decomposition/Isolated Prime\|Isolated Prime]].

Geometrically, isolated primes describe irreducible components, while embedded primes record additional scheme-theoretic or multiplicity structure lying inside those components.

## Example

In $k[x,y]$,

$$
(x^2,xy)=(x)\cap(x^2,y)
$$

has associated primes $(x)$ and $(x,y)$. The line prime $(x)$ is isolated; the point prime $(x,y)$ is embedded.

## Nonuniqueness

The embedded prime itself is intrinsic by the first uniqueness theorem, but its primary component generally is not. For the same ideal,

$$
(x^2,xy)=(x)\cap(x,y)^2
$$

is another minimal decomposition with a different $(x,y)$-primary component.

## Source

- 04_00_primary_decomposition.pdf, discussion after A&M Theorem 4.5 and Remark after Proposition 4.6, printed pp. 52--53.
