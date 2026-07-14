---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Modules/Localization of a Module/","title":"Localization of a Module","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"],"dg-note-properties":{"title":"Localization of a Module","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"],"aliases":["Localized Module"]}}
---


# Localization of a Module
For an $A$-[[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Foundations/Module\|Module]] $M$ and [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Core/Multiplicative Set\|Multiplicative Set]] $S$, the **localized module** $S^{-1}M$ consists of fractions $m/s$ modulo

$$
m/s=m'/s' \quad\Longleftrightarrow\quad
t(s'm-sm')=0\text{ for some }t\in S.
$$

It is naturally an $S^{-1}A$-module, and

$$
S^{-1}M\cong S^{-1}A\otimes_A M.
$$

An element $m/1$ vanishes precisely when some denominator $s\in S$ kills $m$. Thus localization discards the part of $M$ invisible away from $S$.

## Functoriality

An $A$-linear map $f:M\to N$ induces $S^{-1}f:S^{-1}M\to S^{-1}N$ by $m/s\mapsto f(m)/s$. These maps preserve composition and form the localization functor. Its central feature is [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Modules/Exactness of Localization\|Exactness of Localization]].

## Prime localization

For $S=A\setminus\mathfrak p$, write $M_{\mathfrak p}$. The family of modules $M_{\mathfrak p}$ detects whether $M$ is zero and determines the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Localization and Support/Support of a Module\|Support of a Module]].

## Source

- 03_00_rings_and_modules_of_fractions.pdf, A&M Propositions 3.3, 3.5, and 3.7 with Corollaries 3.4 and 3.6, printed pp. 38--40.
