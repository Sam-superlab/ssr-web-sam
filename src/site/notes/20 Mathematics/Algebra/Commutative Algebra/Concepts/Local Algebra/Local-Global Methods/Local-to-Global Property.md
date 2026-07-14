---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Local Algebra/Local-Global Methods/Local-to-Global Property/","title":"Local-to-Global Property","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/local-algebra"],"dg-note-properties":{"title":"Local-to-Global Property","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/local-algebra"],"aliases":["Local Property"]}}
---


# Local-to-Global Property

A property of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$, an $A$-[[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Foundations/Module\|Module]] $M$, or a module homomorphism is **local** when it can be checked after localization. A common algebraic form is

$$
P(M)\quad\Longleftrightarrow\quad
P(M_{\mathfrak p})\text{ for every }\mathfrak p\in\operatorname{Spec}(A).
$$

For many properties it is equivalent to test only maximal ideals. A geometric formulation says that the property may be checked on an open cover of [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Core/Prime Spectrum\|$\operatorname{Spec}(A)$]]. The exact formulation and hypotheses are part of the theorem; “local” is not a universal automatic principle.

## Standard examples

- $M=0$ if and only if $M_{\mathfrak p}=0$ for every prime ideal $\mathfrak p$.
- A module homomorphism is injective, surjective, or an isomorphism if and only if all of its prime localizations have that property.
- Flatness is local: $M$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Flatness and Tor/Flat Module\|Flat Module]] if and only if every $M_{\mathfrak p}$ is flat over $A_{\mathfrak p}$.
- For a domain, being an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Integral Closure and Normality/Integrally Closed Domain\|Integrally Closed Domain]] can be checked at prime or maximal localizations.

## Why localization detects failure

If an element or a cokernel class is nonzero, its annihilator lies in some [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|Prime Ideal]]. Localizing at that prime keeps the obstruction visible. This converts many global equality or exactness questions into statements over [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Local Algebra/Core/Local Ring\|local rings]].

## Caution

Similar-looking statements can fail. For example, every localization of $k\times k$ at a prime ideal is a field, but $k\times k$ is not an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]]. Thus “being a domain” is not a local property for arbitrary rings.

## Source

- `03_01_local_properties.pdf`, A&M Propositions 3.8–3.10, printed pp. 40–41.
