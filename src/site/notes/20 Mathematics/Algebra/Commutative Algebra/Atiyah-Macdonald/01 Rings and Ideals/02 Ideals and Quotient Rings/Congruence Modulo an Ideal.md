---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Congruence Modulo an Ideal/","dg-note-properties":{}}
---


# Congruence Modulo an Ideal

Let $\mathfrak a$ be an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Ideal\|Ideal]] of a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring\|Ring]] $A$. The notation

$$
x\equiv y\pmod{\mathfrak a}
$$

means

$$
x-y\in\mathfrak a.
$$

Equivalently, $x$ and $y$ determine the same element of the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Quotient Ring\|Quotient Ring]] $A/\mathfrak a$.

## Compatibility with operations

If $x\equiv x'\pmod{\mathfrak a}$ and $y\equiv y'\pmod{\mathfrak a}$, then

$$
x+y\equiv x'+y'\pmod{\mathfrak a},
\qquad
xy\equiv x'y'\pmod{\mathfrak a}.
$$

For multiplication,

$$
xy-x'y'=x(y-y')+y'(x-x')\in\mathfrak a.
$$

This calculation is exactly why ideals, rather than arbitrary additive subgroups, define ring quotients.

## Examples

- In $\mathbb Z$, $17\equiv2\pmod{(5)}$ because $15\in(5)$.
- In $k[x]$, $f(x)\equiv f(a)\pmod{(x-a)}$ by the polynomial remainder theorem.
- For a homomorphism $f:A\to B$, $x\equiv y\pmod{\ker f}$ exactly when $f(x)=f(y)$.

## Source

- 01_02_ideals_quotient_rings.pdf, printed p. 2 (notation $x\equiv y\pmod{\mathfrak a}$).

