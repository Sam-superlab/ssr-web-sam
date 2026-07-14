---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Core/Localization of a Ring/","title":"Localization of a Ring","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"],"dg-note-properties":{"title":"Localization of a Ring","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"]}}
---


# Localization of a Ring

Given a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ and a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Core/Multiplicative Set\|Multiplicative Set]] $S$, the **localization** $S^{-1}A$ is the ring obtained by making every element of $S$ invertible.

## Fraction model

Its elements are fractions $a/s$, with equality defined by

$$
a/s=b/t \quad\Longleftrightarrow\quad u(at-bs)=0
\text{ for some }u\in S.
$$

The factor $u$ matters in rings with zero-divisors. The canonical map $A\to S^{-1}A$ has kernel

$$
\{a\in A:sa=0\text{ for some }s\in S\}.
$$

## Universal property

Every homomorphism $A\to B$ that sends $S$ into $B^\times$ factors uniquely through $S^{-1}A$. Consequently, two proposed constructions of localization are canonically isomorphic once they satisfy this property.

## Localization at a prime

For $S=A\setminus\mathfrak p$, write $A_{\mathfrak p}$. Its unique maximal ideal is $\mathfrak pA_{\mathfrak p}$, and its prime ideals correspond to the primes of $A$ contained in $\mathfrak p$; see [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Localization and Support/Prime Correspondence Under Localization\|Prime Correspondence Under Localization]].

## Example

For $A=\mathbb Z$ and $S=\mathbb Z\setminus(p)$, $A_{(p)}$ consists of rational numbers whose denominators are not divisible by $p$. This differs from $\mathbb Z[1/p]$, where only powers of $p$ are allowed in denominators.

## Source

- 03_00_rings_and_modules_of_fractions.pdf, A&M Proposition 3.1 and examples, printed pp. 36--38.
