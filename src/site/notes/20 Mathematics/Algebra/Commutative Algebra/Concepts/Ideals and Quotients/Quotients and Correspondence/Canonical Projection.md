---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Canonical Projection/","title":"Canonical Projection","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Canonical Projection","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Canonical Projection

For an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] $\mathfrak a\subseteq A$, the **canonical projection** is

$$
\pi:A\to A/\mathfrak a,\qquad \pi(x)=x+\mathfrak a.
$$

It is a surjective [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring Homomorphism\|Ring Homomorphism]] with

$$
\ker\pi=\mathfrak a.
$$

This map packages the meaning of the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Quotient Ring\|Quotient Ring]]: two elements have the same image precisely when their difference lies in $\mathfrak a$.

## Universal property

If $f:A\to B$ is a ring homomorphism satisfying $\mathfrak a\subseteq\ker f$, then there is a unique homomorphism

$$
\bar f:A/\mathfrak a\to B
$$

such that $f=\bar f\circ\pi$. It is defined by $\bar f(x+\mathfrak a)=f(x)$. The kernel condition is exactly what makes this definition independent of the representative.

## Example

The reduction map $\mathbb Z\to\mathbb Z/n\mathbb Z$ is the canonical projection for the ideal $(n)$.

The projection is the map used in the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Correspondence Theorem for Ideals\|Correspondence Theorem for Ideals]] and the model for all surjective ring homomorphisms via the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/First Isomorphism Theorem for Rings\|First Isomorphism Theorem for Rings]].

## Source

- 01_02_ideals_quotient_rings.pdf, printed p. 2 (natural surjection $A\to A/\mathfrak a$).

