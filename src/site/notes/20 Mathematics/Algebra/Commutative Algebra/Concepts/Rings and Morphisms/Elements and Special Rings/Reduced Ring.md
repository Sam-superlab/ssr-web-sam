---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Reduced Ring/","title":"Reduced Ring","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"],"dg-note-properties":{"title":"Reduced Ring","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"]}}
---


# Reduced Ring

A [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ is **reduced** if it has no nonzero [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Nilpotent Element\|nilpotent elements]]. Equivalently,

$$
\sqrt{(0)}=(0),
$$

so its [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Nilradical\|Nilradical]] is zero.

## Examples and nonexamples

- Every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]] is reduced.
- $\mathbb Z/n\mathbb Z$ is reduced exactly when $n$ is squarefree.
- $k[x,y]/(xy)$ is reduced but not a domain: the classes of $x$ and $y$ are nonzero zero divisors, yet there are no nonzero nilpotents.
- $k[\varepsilon]/(\varepsilon^2)$ is not reduced.

## Reduction of a ring

For every ring $A$, the quotient

$$
A_{\mathrm{red}}=A/\operatorname{Nil}(A)
$$

is reduced. If the class of $x$ in this quotient is nilpotent, then $x^n$ lies in the nilradical; some further power of $x$ is zero, so $x$ was already in the nilradical.

By [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Nilradical\|Proposition 1.8]], a ring is reduced exactly when the intersection of all its [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|prime ideals]] is zero.

## Source

- 01_05_nilradical_jacobson_radical.pdf, printed p. 5; Proposition 1.7 (the quotient by the nilradical has no nonzero nilpotents).

