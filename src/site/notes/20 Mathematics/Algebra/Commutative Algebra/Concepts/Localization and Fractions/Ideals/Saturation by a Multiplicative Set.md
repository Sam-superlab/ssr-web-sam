---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Ideals/Saturation by a Multiplicative Set/","title":"Saturation by a Multiplicative Set","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"],"dg-note-properties":{"title":"Saturation by a Multiplicative Set","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"],"aliases":["Saturation of an Ideal"]}}
---


# Saturation by a Multiplicative Set
For an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] $\mathfrak a\subseteq A$ and [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Core/Multiplicative Set\|Multiplicative Set]] $S$, its **saturation with respect to $S$** is

$$
S(\mathfrak a)=\{x\in A:sx\in\mathfrak a\text{ for some }s\in S\}.
$$

Equivalently, it is the contraction of $S^{-1}\mathfrak a$ along $A\to S^{-1}A$, so $S(\mathfrak a)=\mathfrak a^{ec}$.

## Properties

- $S(\mathfrak a)=(1)$ exactly when $S\cap\mathfrak a\ne\varnothing$.
- Saturation commutes with radicals and finite intersections.
- Repeated saturation satisfies $S_1(S_2(\mathfrak a))=(S_1S_2)(\mathfrak a)$.
- If $S$ consists of powers of $f$, then $S(\mathfrak a)=\bigcup_{n\ge0}(\mathfrak a:f^n)$.

When $\mathfrak a$ has a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Primary Decomposition and Associated Primes/Primary Ideals and Decompositions/Primary Decomposition\|Primary Decomposition]], saturation deletes precisely the primary components whose radicals meet $S$.

## Source

- 03_02_extended_contracted_ideals_fractions.pdf, A&M Proposition 3.11(ii), printed pp. 41--42.
- 04_01_exercises.pdf, A&M Chapter 4, Exercise 12, printed p. 56.
