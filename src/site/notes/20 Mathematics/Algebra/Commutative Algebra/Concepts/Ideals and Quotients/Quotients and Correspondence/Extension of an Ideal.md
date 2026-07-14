---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Extension of an Ideal/","title":"Extension of an Ideal","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Extension of an Ideal","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Extension of an Ideal

Let $f:A\to B$ be a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring Homomorphism\|Ring Homomorphism]] and let $\mathfrak a$ be an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] of $A$. The **extension** of $\mathfrak a$ to $B$ is

$$
\mathfrak a^e
=
Bf(\mathfrak a)
=
\left\{
\sum_{i=1}^r b_i f(a_i):
b_i\in B,\ a_i\in\mathfrak a
\right\}.
$$

It is the smallest ideal of $B$ containing $f(\mathfrak a)$.

## Why generation is necessary

The set $f(\mathfrak a)$ need not absorb multiplication by arbitrary elements of $B$. Under $\mathbb Z\hookrightarrow\mathbb Q$, the image of $(2)$ is $2\mathbb Z$, not an ideal of $\mathbb Q$, while its extension is all of $\mathbb Q$ because $1=(1/2)\cdot2$.

Thus a proper ideal, even a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|Prime Ideal]], can extend to the unit ideal.

## Properties

For ideals $\mathfrak a_1,\mathfrak a_2\subseteq A$,

$$
(\mathfrak a_1+\mathfrak a_2)^e
=
\mathfrak a_1^e+\mathfrak a_2^e,
$$

$$
(\mathfrak a_1\mathfrak a_2)^e
=
\mathfrak a_1^e\mathfrak a_2^e.
$$

Intersections satisfy only

$$
(\mathfrak a_1\cap\mathfrak a_2)^e
\subseteq
\mathfrak a_1^e\cap\mathfrak a_2^e
$$

in general.

Extension is paired with [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Contraction of an Ideal\|contraction]] by the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Extension-Contraction Correspondence\|Extension-Contraction Correspondence]].

## Source

- 01_07_extension_and_contraction.pdf, printed pp. 9-10 (definition, examples, Proposition 1.17, and Exercise 1.18).

