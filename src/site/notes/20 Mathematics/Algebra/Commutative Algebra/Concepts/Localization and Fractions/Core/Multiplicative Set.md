---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Core/Multiplicative Set/","title":"Multiplicative Set","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"],"dg-note-properties":{"title":"Multiplicative Set","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"]}}
---


# Multiplicative Set

A **multiplicative set** in a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ is a subset $S\subseteq A$ such that $1\in S$ and $st\in S$ whenever $s,t\in S$. It specifies which elements become invertible in [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Core/Localization of a Ring\|localization]].

## Examples

- $\{1,f,f^2,\ldots\}$ localizes at one element.
- $A\setminus\mathfrak p$ is multiplicative exactly when $\mathfrak p$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|Prime Ideal]].
- The set of all non-zero-divisors gives the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Fraction Rings/Total Ring of Fractions\|Total Ring of Fractions]].
- $1+\mathfrak a=\{1+x:x\in\mathfrak a\}$ is multiplicative.

If $0\in S$, every fraction equals zero, so $S^{-1}A$ is the zero ring. This edge case often turns a claim about proper ideals into a condition that an ideal avoid $S$.

## Saturation

A multiplicative set is saturated when $xy\in S$ holds exactly when both $x$ and $y$ lie in $S$. Saturating $S$ does not change the localization; it records every element that already becomes a unit in $S^{-1}A$.

## Source

- 03_00_rings_and_modules_of_fractions.pdf, A&M Chapter 3, printed pp. 36--38.
