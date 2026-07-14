---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Ideals/Extension and Contraction Under Localization/","title":"Extension and Contraction Under Localization","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"],"dg-note-properties":{"title":"Extension and Contraction Under Localization","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"]}}
---


# Extension and Contraction Under Localization

For the map $A\to S^{-1}A$, extend an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] $\mathfrak a\subseteq A$ to $S^{-1}\mathfrak a$ and contract an ideal $\mathfrak b\subseteq S^{-1}A$ by inverse image.

## The special feature

Every ideal upstairs is extended:

$$
\mathfrak b=(\mathfrak b^c)^e.
$$

Downstairs, extension followed by contraction gives the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Ideals/Saturation by a Multiplicative Set\|Saturation by a Multiplicative Set]]:

$$
\mathfrak a^{ec}=\{x\in A:sx\in\mathfrak a\text{ for some }s\in S\}.
$$

Therefore distinct ideals of $A$ can have the same extension; localization forgets the difference measured by $S$-torsion.

## Properness

$S^{-1}\mathfrak a$ is proper if and only if $\mathfrak a$ is disjoint from $S$. This criterion drives the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Localization and Support/Prime Correspondence Under Localization\|Prime Correspondence Under Localization]].

## Source

- 03_02_extended_contracted_ideals_fractions.pdf, A&M Proposition 3.11, printed pp. 41--42.
