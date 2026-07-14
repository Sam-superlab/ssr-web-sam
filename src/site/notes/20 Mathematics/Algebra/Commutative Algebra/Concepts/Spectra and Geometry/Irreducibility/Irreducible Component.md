---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Irreducibility/Irreducible Component/","title":"Irreducible Component","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/spectra-and-geometry"],"dg-note-properties":{"title":"Irreducible Component","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/spectra-and-geometry"]}}
---


# Irreducible Component

An **irreducible component** of a topological space is a maximal [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Irreducibility/Irreducible Topological Space\|irreducible]] subspace. Every irreducible component is closed, and the components cover the space.

For the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Core/Prime Spectrum\|Prime Spectrum]] of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$, the irreducible components are exactly

$$
V(\mathfrak p)
$$

where $\mathfrak p$ runs over the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Minimal Prime Ideal\|minimal prime ideals]] of $A$.

## Why minimal primes appear

The closed set $V(\mathfrak p)$ is irreducible when $\mathfrak p$ is prime. Inclusion reverses:

$$
V(\mathfrak p)\subseteq V(\mathfrak q)
\iff
\mathfrak q\subseteq\mathfrak p.
$$

Therefore maximal irreducible closed subsets correspond exactly to prime ideals minimal under inclusion.

## Examples

- If $A$ is an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]], $\operatorname{Spec}(A)$ has one irreducible component, since $(0)$ is its unique minimal prime.
- For $A=k[x,y]/(xy)$, the spectrum has two components, $V(x)$ and $V(y)$, reflecting the two coordinate axes.
- A Hausdorff space has only one-point irreducible subspaces, so its irreducible components are singletons.

## Source

- 01_08_exercises.pdf, printed p. 13; Exercise 20.

