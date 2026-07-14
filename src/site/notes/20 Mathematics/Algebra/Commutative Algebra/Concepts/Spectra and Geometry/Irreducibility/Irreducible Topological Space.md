---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Irreducibility/Irreducible Topological Space/","title":"Irreducible Topological Space","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/spectra-and-geometry"],"dg-note-properties":{"title":"Irreducible Topological Space","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/spectra-and-geometry"]}}
---


# Irreducible Topological Space

A nonempty topological space $X$ is **irreducible** if any two nonempty open subsets intersect. Equivalently, every nonempty open subset is dense, or $X$ cannot be written as the union of two proper closed subsets.

## Spectral criterion

For a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$,

$$
\operatorname{Spec}(A)\text{ is irreducible}
\iff
\operatorname{Nil}(A)\text{ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|Prime Ideal]]}.
$$

Equivalently, the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Reduced Ring\|Reduced Ring]] $A/\operatorname{Nil}(A)$ is an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]].

To see the connection, if $D(f)$ and $D(g)$ are nonempty basic opens but disjoint, then $D(fg)=\varnothing$, so $fg$ is nilpotent. Primality of the nilradical would force $f$ or $g$ to be nilpotent, making one of the original opens empty.

## Generic points

For a prime ideal $\mathfrak p$, the closed subset $V(\mathfrak p)$ is irreducible, and the point $\mathfrak p$ is dense in it:

$$
\overline{\{\mathfrak p\}}=V(\mathfrak p).
$$

Such a point is called a generic point. Maximal irreducible closed subsets are the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Irreducibility/Irreducible Component\|irreducible components]].

## Source

- 01_08_exercises.pdf, printed p. 13; Exercises 19-20.
