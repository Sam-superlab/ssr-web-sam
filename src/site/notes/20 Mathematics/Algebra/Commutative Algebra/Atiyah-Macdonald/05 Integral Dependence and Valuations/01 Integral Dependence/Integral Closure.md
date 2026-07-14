---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/05 Integral Dependence and Valuations/01 Integral Dependence/Integral Closure/","dg-note-properties":{}}
---


# Integral Closure

For $A\subseteq B$, the **integral closure of $A$ in $B$** is the set

$$
\overline A^{,B}=\{x\in B:x\text{ is integral over }A\}.
$$

It is a subring of $B$ containing $A$. It is integrally closed in $B$: an element of $B$ integral over the closure is already integral over $A$ by transitivity.

## Examples

- The integral closure of $\mathbb Z$ in $\mathbb Q$ is $\mathbb Z$.
- The integral closure of $k[t^2,t^3]$ in $k(t)$ is $k[t]$.
- For a domain, its integral closure in its fraction field is its normalization; equality defines an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/05 Integral Dependence and Valuations/03 Going Down/Integrally Closed Domain\|Integrally Closed Domain]].

## Localization

Integral closure commutes with [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/03 Rings and Modules of Fractions/01 Localization/Localization of a Ring\|localization]]: if $C$ is the integral closure of $A$ in $B$, then $S^{-1}C$ is the integral closure of $S^{-1}A$ in $S^{-1}B$.

## Valuative description

Inside a field $K$, the integral closure of $A$ equals the intersection of all [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/05 Integral Dependence and Valuations/04 Valuation Rings/Valuation Ring\|valuation rings]] of $K$ containing $A$; see [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/05 Integral Dependence and Valuations/04 Valuation Rings/Valuative Criterion for Integral Closure\|Valuative Criterion for Integral Closure]].

## Source

- 05_01_integral_dependence.pdf, A&M Corollaries 5.3 and 5.5, printed pp. 60--61.
- 05_03_integrally_closed_going_down.pdf, A&M Proposition 5.12, printed pp. 62--63.
- 05_04_valuation_rings.pdf, A&M Corollary 5.22, printed p. 66.
