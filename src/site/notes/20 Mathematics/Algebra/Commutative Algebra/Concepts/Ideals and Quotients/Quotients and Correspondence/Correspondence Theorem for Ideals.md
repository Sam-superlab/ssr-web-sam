---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Correspondence Theorem for Ideals/","title":"Correspondence Theorem for Ideals","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Correspondence Theorem for Ideals","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Correspondence Theorem for Ideals

Let $\mathfrak a$ be an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] of $A$, and let $\pi:A\to A/\mathfrak a$ be the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Canonical Projection\|Canonical Projection]]. There is an inclusion-preserving bijection

$$
\{\mathfrak b\triangleleft A:\mathfrak a\subseteq\mathfrak b\}
\longleftrightarrow
\{\text{ideals of }A/\mathfrak a\}.
$$

The maps are

$$
\mathfrak b\longmapsto\mathfrak b/\mathfrak a,
\qquad
\mathfrak c\longmapsto\pi^{-1}(\mathfrak c).
$$

These operations are inverse because $\pi$ is surjective.

## Why it works

Every ideal of a quotient has a full inverse image in $A$, and that inverse image must contain $\ker\pi=\mathfrak a$. Conversely, if $\mathfrak b$ contains $\mathfrak a$, its image $\mathfrak b/\mathfrak a$ is closed under addition and absorbs multiplication in the quotient.

## Consequences

- Ideals strictly between $\mathfrak a$ and $A$ correspond to nonzero proper ideals of $A/\mathfrak a$.
- $\mathfrak a$ is [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Maximal Ideal\|maximal]] exactly when $A/\mathfrak a$ has no ideals except $(0)$ and $(1)$, hence is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Field\|Field]].
- Prime ideals of $A/\mathfrak a$ correspond to prime ideals of $A$ containing $\mathfrak a$.

## Example

Ideals of $\mathbb Z/(12)$ correspond to ideals $(d)$ of $\mathbb Z$ containing $(12)$, equivalently divisors $d$ of $12$.

## Source

- 01_02_ideals_quotient_rings.pdf, printed p. 2; Proposition 1.1.

