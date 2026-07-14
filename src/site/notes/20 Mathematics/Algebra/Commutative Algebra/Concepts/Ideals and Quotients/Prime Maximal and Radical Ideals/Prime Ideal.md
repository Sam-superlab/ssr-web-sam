---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal/","title":"Prime Ideal","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Prime Ideal","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Prime Ideal

A **prime ideal** $\mathfrak p$ of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ is a proper [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] such that

$$
xy\in\mathfrak p
\quad\Longrightarrow\quad
x\in\mathfrak p\text{ or }y\in\mathfrak p.
$$

The condition extends to finite products: if $x_1\cdots x_n\in\mathfrak p$, then some $x_i\in\mathfrak p$.

## Quotient characterization

$$
\mathfrak p\text{ is prime}
\iff
A/\mathfrak p\text{ is an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]]}.
$$

Indeed, $(x+\mathfrak p)(y+\mathfrak p)=0$ exactly when $xy\in\mathfrak p$.

## Examples and nonexamples

- $(0)$ is prime in $\mathbb Z$.
- $(p)$ is prime in $\mathbb Z$ for a prime number $p$.
- If $f\in k[x_1,\ldots,x_n]$ is irreducible, $(f)$ is prime because the polynomial ring is a unique factorization domain.
- $(6)$ is not prime in $\mathbb Z$: $2\cdot3\in(6)$ but neither factor lies in $(6)$.

Every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Maximal Ideal\|Maximal Ideal]] is prime, but $(0)\subset\mathbb Z$ shows the converse fails.

## Contraction

If $f:A\to B$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring Homomorphism\|Ring Homomorphism]] and $\mathfrak q$ is prime in $B$, then

$$
f^{-1}(\mathfrak q)
$$

is prime in $A$. This is the basic functorial behavior behind the map on [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Core/Prime Spectrum\|prime spectra]].

## Source

- 01_04_prime_and_maximal_ideals.pdf, printed p. 3 (definition, quotient test, and contraction).

