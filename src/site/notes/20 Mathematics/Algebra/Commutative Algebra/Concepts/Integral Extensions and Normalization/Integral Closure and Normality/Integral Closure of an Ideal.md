---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Integral Closure and Normality/Integral Closure of an Ideal/","title":"Integral Closure of an Ideal","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/integral-extensions-and-normalization"],"dg-note-properties":{"title":"Integral Closure of an Ideal","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/integral-extensions-and-normalization"]}}
---


# Integral Closure of an Ideal

Let $I$ be an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$. An element $x\in A$ is **integral over $I$** if it satisfies an equation

$$
x^n+a_1x^{n-1}+\cdots+a_n=0
$$

with


$$
a_i\in I^i\qquad(1\le i\le n).
$$

The set of all elements integral over $I$ is an ideal called the **integral closure of $I$**, denoted $\overline I$. The ideal is **integrally closed** if $I=\overline I$.

## Basic properties

For ideals $I\subseteq J$,

$$
I\subseteq\overline I,\qquad
\overline{\overline I}=\overline I,\qquad
\sqrt{\overline I}=\sqrt I,\qquad
\overline I\subseteq\overline J.
$$

The powers $I^i$ in the coefficient condition are essential. Replacing every $I^i$ by $I$ gives a different construction related to [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Integral Closure and Normality/Radical of an Extended Ideal under Integral Closure\|the radical of an extended ideal]].

## Example

In $k[x,y]$,

$$
\overline{(x^2,y^2)}=(x^2,xy,y^2).
$$

Indeed, $(xy)^2-x^2y^2=0$ is an integral equation over $(x^2,y^2)$, and the resulting ideal is the degree-two monomial ideal $(x,y)^2$.

## Rees-algebra viewpoint

The element $x$ is integral over $I$ exactly when $xt$ is integral over the Rees algebra $A[It]$ inside $A[t]$. This packages the powers $I^i$ into the grading and connects ideal integral closure with blowups and asymptotic ideal theory.

## Source

- Standard definition, added to distinguish ideal integral closure from the coefficient condition in A&M Lemma 5.14.
