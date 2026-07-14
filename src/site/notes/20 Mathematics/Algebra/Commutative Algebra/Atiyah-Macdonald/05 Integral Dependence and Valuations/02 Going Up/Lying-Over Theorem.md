---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/05 Integral Dependence and Valuations/02 Going Up/Lying-Over Theorem/","dg-note-properties":{}}
---


# Lying-Over Theorem

If $A\subseteq B$ is an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/05 Integral Dependence and Valuations/01 Integral Dependence/Integral Extension\|Integral Extension]], then for every prime ideal $\mathfrak p$ of $A$ there exists a prime ideal $\mathfrak q$ of $B$ such that

$$
\mathfrak q\cap A=\mathfrak p.
$$

Equivalently, the contraction map $\operatorname{Spec}B\to\operatorname{Spec}A$ is surjective.

## Proof sketch

Localize both rings at $A\setminus\mathfrak p$. The extension remains integral. A maximal ideal of the localized $B$ contracts to a maximal ideal of the local ring $A_{\mathfrak p}$, necessarily $\mathfrak pA_{\mathfrak p}$. Contracting back to $B$ produces the desired prime.

## Role

Lying over starts the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/05 Integral Dependence and Valuations/02 Going Up/Going-Up Theorem\|Going-Up Theorem]] and explains why integral morphisms do not omit base primes.

## Source

- 05_02_going_up_theorem.pdf, A&M Theorem 5.10, printed p. 62.
