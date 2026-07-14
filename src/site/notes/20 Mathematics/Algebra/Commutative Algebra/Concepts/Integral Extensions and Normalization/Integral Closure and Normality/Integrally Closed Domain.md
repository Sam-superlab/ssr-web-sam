---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Integral Closure and Normality/Integrally Closed Domain/","title":"Integrally Closed Domain","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/integral-extensions-and-normalization"],"dg-note-properties":{"title":"Integrally Closed Domain","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/integral-extensions-and-normalization"]}}
---


# Integrally Closed Domain

An integral domain $A$ is **integrally closed** if every element of its [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Fraction Rings/Field of Fractions\|Field of Fractions]] that is integral over $A$ already belongs to $A$.

Equivalently, $A$ equals its [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Integral Closure and Normality/Integral Closure\|Integral Closure]] in its fraction field. Such a domain is also called a **normal domain**; Noetherianity is not part of this definition, although many geometric theorems impose it separately.

## Examples

- $\mathbb Z$ is integrally closed.
- Every unique factorization domain is integrally closed.
- Therefore $k[x_1,\ldots,x_n]$ is integrally closed when $k$ is a field.
- $k[t^2,t^3]$ is not integrally closed in $k(t)$ because $t$ is integral over it but is not in it.
- Every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Valuation Theory/Valuation Rings and Integral Closure/Valuation Ring\|Valuation Ring]] is integrally closed.

## Local criterion

$A$ is integrally closed exactly when every $A_{\mathfrak p}$ is integrally closed, equivalently every $A_{\mathfrak m}$ for maximal $\mathfrak m$ is integrally closed.

## Role in going down

An integrally closed base is the key extra hypothesis in the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Prime Spectra under Integral Extensions/Going-Down Theorem\|Going-Down Theorem]] for integral extensions of domains.

## Source

- 05_03_integrally_closed_going_down.pdf, A&M Propositions 5.12--5.13, printed pp. 62--63.
