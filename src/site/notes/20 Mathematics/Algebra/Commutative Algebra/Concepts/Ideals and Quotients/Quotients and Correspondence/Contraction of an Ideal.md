---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Contraction of an Ideal/","title":"Contraction of an Ideal","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Contraction of an Ideal","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Contraction of an Ideal

Let $f:A\to B$ be a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring Homomorphism\|Ring Homomorphism]] and let $\mathfrak b$ be an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] of $B$. The **contraction** of $\mathfrak b$ to $A$ is

$$
\mathfrak b^c=f^{-1}(\mathfrak b).
$$

Unlike the direct image of an ideal, an inverse image is automatically an ideal.

## Prime ideals contract

If $\mathfrak q$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|Prime Ideal]] of $B$, then $\mathfrak q^c$ is prime in $A$. If $xy\in f^{-1}(\mathfrak q)$, then $f(x)f(y)\in\mathfrak q$, so $f(x)$ or $f(y)$ lies in $\mathfrak q$.

Contraction does not preserve maximality. For $\mathbb Z\hookrightarrow\mathbb Q$, the maximal ideal $(0)$ of $\mathbb Q$ contracts to $(0)$ in $\mathbb Z$, which is prime but not [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Maximal Ideal\|maximal]].

## Properties

For ideals $\mathfrak b_1,\mathfrak b_2\subseteq B$,

$$
(\mathfrak b_1\cap\mathfrak b_2)^c
=
\mathfrak b_1^c\cap\mathfrak b_2^c,
$$

while

$$
\mathfrak b_1^c+\mathfrak b_2^c
\subseteq
(\mathfrak b_1+\mathfrak b_2)^c
$$

and

$$
\mathfrak b_1^c\mathfrak b_2^c
\subseteq
(\mathfrak b_1\mathfrak b_2)^c
$$

may be strict.

Contraction is paired with [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Extension of an Ideal\|extension]] by the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Extension-Contraction Correspondence\|Extension-Contraction Correspondence]].

## Source

- 01_07_extension_and_contraction.pdf, printed pp. 9-10 (definition, prime contraction, Proposition 1.17, and Exercise 1.18).

