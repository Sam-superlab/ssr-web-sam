---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Sources/Atiyah-Macdonald/01 Rings and Ideals/08 Exercises and Further Directions/08 Exercises and Further Directions/","title":"08 Exercises and Further Directions","tags":["mathematics/commutative-algebra","source/textbook/atiyah-macdonald"],"dg-note-properties":{"title":"08 Exercises and Further Directions","type":"source-note","tags":["mathematics/commutative-algebra","source/textbook/atiyah-macdonald"]}}
---


# Exercises and Further Directions

The Chapter 1 exercises do more than test definitions. They develop several themes that become central later.

## Element tests and special rings

Exercises 1-12 sharpen the behavior of [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Nilpotent Element\|nilpotents]], [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Unit\|units]], and [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Zero Divisor\|zero divisors]] in polynomial and power-series rings. They also introduce [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Idempotent\|idempotents]] and [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Boolean Ring\|Boolean rings]], and relate unique prime ideals to the quotient by the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Nilradical\|Nilradical]].

Useful patterns include:

- $1+x$ is a unit when $x$ is nilpotent;
- a polynomial is a unit precisely when its constant term is a unit and its other coefficients are nilpotent;
- every prime ideal contains a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Minimal Prime Ideal\|minimal prime ideal]];
- a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Local Algebra/Core/Local Ring\|Local Ring]] has no idempotents except $0$ and $1$.

## Existence by maximal ideals

Exercise 13 constructs an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Fields and Extensions/Core/Artin Construction of an Algebraic Closure\|Artin Construction of an Algebraic Closure]] by adjoining formal roots, placing the resulting relations inside a maximal ideal, and iterating.

Exercise 14 studies maximal ideals consisting entirely of zero divisors and concludes that the set of zero divisors is a union of prime ideals.

## The prime spectrum

Exercises 15-25 introduce the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Core/Prime Spectrum\|Prime Spectrum]]

$$
\operatorname{Spec}(A)=\{\mathfrak p:\mathfrak p\text{ prime}\}
$$

and the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Core/Zariski Topology\|Zariski Topology]]. Its [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Core/Basic Open Set\|basic open sets]] $D(f)$ are quasi-compact and form a basis. Algebra becomes topology:

- closed points correspond to [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Maximal Ideal\|maximal ideals]];
- $\operatorname{Spec}(A)$ is irreducible exactly when the nilradical is prime;
- [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Irreducibility/Irreducible Component\|irreducible components]] correspond to minimal primes;
- nontrivial idempotents correspond to decompositions of the spectrum.

Boolean rings connect this picture to compact Hausdorff totally disconnected spaces and Stone duality.

## Maximal spectra and varieties

Exercise 26 defines the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Core/Maximal Spectrum\|Maximal Spectrum]] and reconstructs a compact Hausdorff space $X$ from the maximal ideals of $C(X)$.

Exercises 27-28 introduce an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Affine Geometry/Affine Algebraic Set\|Affine Algebraic Set]], its [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Affine Geometry/Coordinate Ring\|Coordinate Ring]], and [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Affine Geometry/Regular Map\|regular maps]]. A regular map $X\to Y$ induces a homomorphism in the opposite direction:

$$
P(Y)\to P(X).
$$

This contravariance is a first glimpse of the algebra-geometry dictionary.

## Source

- 01_08_exercises.pdf, printed pp. 10-16; Exercises 1-28.
