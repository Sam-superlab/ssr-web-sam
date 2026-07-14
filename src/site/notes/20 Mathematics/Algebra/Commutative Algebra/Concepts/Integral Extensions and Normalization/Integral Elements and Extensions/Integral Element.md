---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Integral Elements and Extensions/Integral Element/","title":"Integral Element","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/integral-extensions-and-normalization"],"dg-note-properties":{"title":"Integral Element","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/integral-extensions-and-normalization"]}}
---


# Integral Element

For a ring extension $A\subseteq B$, an element $x\in B$ is **integral over $A$** if it is a root of a monic polynomial in $A[T]$:

$$
x^n+a_1x^{n-1}+\cdots+a_n=0.
$$

## Equivalent finite condition

$x$ is integral exactly when $A[x]$ is finitely generated as an $A$-[[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Foundations/Module\|Module]]. The monic equation bounds the required powers by $1,x,\ldots,x^{n-1}$; conversely, the determinant trick produces a monic equation from a finite stable module.

## Examples

- Every element of $A$ is integral over $A$.
- $\sqrt d$ is integral over $\mathbb Z$ because it satisfies $T^2-d$.
- A rational number integral over $\mathbb Z$ is an integer.
- In $k(t)$, the element $t$ is integral over $k[t^2,t^3]$ because $t^2$ lies in the smaller ring and $t$ satisfies $T^2-t^2$.

## Caution

The adjective is relative to a base ring. The same element may be integral over one subring and not over another.

## Source

- 05_01_integral_dependence.pdf, A&M Example 5.0 and Proposition 5.1, printed pp. 59--60.
