---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Nilpotent Element/","title":"Nilpotent Element","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"],"dg-note-properties":{"title":"Nilpotent Element","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/rings-and-morphisms"]}}
---


# Nilpotent Element

An element $x$ of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ is **nilpotent** if

$$
x^n=0
$$

for some integer $n>0$. The least such $n$, when $x\neq0$, is sometimes called the nilpotency index.

## Examples and nonexamples

- In $k[\varepsilon]/(\varepsilon^2)$, the class of $\varepsilon$ is nonzero and nilpotent.
- In $\mathbb Z/8\mathbb Z$, the class of $2$ is nilpotent because $2^3=0$.
- The class of $2$ in $\mathbb Z/6\mathbb Z$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Zero Divisor\|Zero Divisor]] but is not nilpotent.
- An [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]] has no nonzero nilpotents.

Every nonzero nilpotent is a zero divisor. Nilpotents are never [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Unit\|units]] in a nonzero ring: if $x^n=0$ and $x$ were invertible, then $1=x^{-n}x^n=0$.

## Stability properties

In a commutative ring, the sum of two nilpotent elements is nilpotent. If $x^m=0$ and $y^n=0$, every term in the binomial expansion of $(x+y)^{m+n-1}$ vanishes. Also $ax$ is nilpotent for every $a\in A$.

Therefore all nilpotent elements form the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Nilradical\|Nilradical]]. Passing to $A/\sqrt{(0)}$ removes every nonzero nilpotent and produces a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Reduced Ring\|Reduced Ring]].

## Source

- 01_03_zero_divisors_nilpotent_units.pdf, printed p. 2 (definition).
- 01_05_nilradical_jacobson_radical.pdf, printed p. 5 (Proposition 1.7: the nilpotent elements form an ideal).
