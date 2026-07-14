---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Finite Prime Avoidance/","title":"Finite Prime Avoidance","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Finite Prime Avoidance","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"aliases":["Prime Avoidance"]}}
---


# Finite Prime Avoidance
The finite **prime avoidance** result has two complementary forms.

## Avoiding a finite union

Let $\mathfrak p_1,\ldots,\mathfrak p_n$ be [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|prime ideals]]. If an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] $\mathfrak a$ satisfies

$$
\mathfrak a\subseteq\bigcup_{i=1}^n\mathfrak p_i,
$$

then

$$
\mathfrak a\subseteq\mathfrak p_i
$$

for some $i$.

In contrapositive form: if $\mathfrak a$ is not contained in any one $\mathfrak p_i$, there is a single element of $\mathfrak a$ that avoids all of them.

## A prime containing an intersection

If a prime ideal $\mathfrak p$ contains

$$
\bigcap_{i=1}^n\mathfrak a_i,
$$

then $\mathfrak p$ contains at least one $\mathfrak a_i$. This follows because $\prod_i\mathfrak a_i$ lies in the intersection and primality forces one factor into $\mathfrak p$.

If moreover $\mathfrak p=\bigcap_i\mathfrak a_i$, then $\mathfrak p=\mathfrak a_i$ for some $i$.

## Why it matters

Prime avoidance lets one choose elements with simultaneous nonmembership conditions. The finiteness of the family is essential to this elementary form.

## Source

- 01_06_operations_on_ideals.pdf, printed p. 8; Proposition 1.11.

