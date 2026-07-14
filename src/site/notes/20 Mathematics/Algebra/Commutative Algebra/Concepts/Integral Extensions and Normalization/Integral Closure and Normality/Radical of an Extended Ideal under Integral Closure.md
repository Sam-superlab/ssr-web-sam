---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Integral Closure and Normality/Radical of an Extended Ideal under Integral Closure/","title":"Radical of an Extended Ideal under Integral Closure","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/integral-extensions-and-normalization"],"dg-note-properties":{"title":"Radical of an Extended Ideal under Integral Closure","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/integral-extensions-and-normalization"]}}
---


# Radical of an Extended Ideal under Integral Closure

Let $A\subseteq B$, let $C$ be the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Integral Closure and Normality/Integral Closure\|Integral Closure]] of $A$ in $B$, and let $\mathfrak a$ be an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] of $A$. For $x\in B$, the following are equivalent:

1. $x\in\sqrt{\mathfrak aC}$;
2. $x$ satisfies an equation

$$
x^n+a_1x^{n-1}+\cdots+a_n=0
$$

with every coefficient $a_i\in\mathfrak a$.

The coefficient condition first implies that $x$ is integral over $A$, hence $x\in C$. The equation then places a power of $x$ in $\mathfrak aC$. Conversely, membership in the radical can be converted into such an equation by collecting finitely many integral coefficients and applying the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Finite Generation and Local Methods/Determinant Trick\|Determinant Trick]].

## Distinction from integral closure of an ideal

This result uses the same coefficient ideal $\mathfrak a$ in every degree. It is **not** the standard definition of the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Integral Closure and Normality/Integral Closure of an Ideal\|Integral Closure of an Ideal]], where the coefficient of $x^{n-i}$ must lie in $\mathfrak a^i$. In general, the integral closure of an ideal is not its radical.

## Source

- `05_03_integrally_closed_going_down.pdf`, A&M Lemma 5.14, printed p. 63.
