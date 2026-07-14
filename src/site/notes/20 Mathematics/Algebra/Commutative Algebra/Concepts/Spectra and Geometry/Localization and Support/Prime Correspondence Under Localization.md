---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Localization and Support/Prime Correspondence Under Localization/","title":"Prime Correspondence Under Localization","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/spectra-and-geometry"],"dg-note-properties":{"title":"Prime Correspondence Under Localization","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/spectra-and-geometry"]}}
---


# Prime Correspondence Under Localization

For a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Core/Multiplicative Set\|Multiplicative Set]] $S\subseteq A$, extension and contraction give inverse bijections

$$
\operatorname{Spec}(S^{-1}A)
\longleftrightarrow
\{\mathfrak p\in\operatorname{Spec}A:\mathfrak p\cap S=\varnothing\}.
$$

The maps are $\mathfrak q\mapsto\mathfrak q^c$ and $\mathfrak p\mapsto S^{-1}\mathfrak p$.

## At a prime

If $S=A\setminus\mathfrak p$, disjointness means $\mathfrak q\subseteq\mathfrak p$. Hence

$$
\operatorname{Spec}(A_{\mathfrak p})
\cong\{\mathfrak q\in\operatorname{Spec}A:\mathfrak q\subseteq\mathfrak p\}.
$$

The maximal ideal of $A_{\mathfrak p}$ corresponds to $\mathfrak p$ itself.

## Geometric reading

For $S=\{1,f,f^2,\ldots\}$, the image is the basic open set $D(f)$: precisely the primes not containing $f$.

## Source

- 03_02_extended_contracted_ideals_fractions.pdf, A&M Proposition 3.11(iv) and Corollary 3.13, printed p. 42.
