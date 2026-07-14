---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Jacobson Radical Unit Test/","title":"Jacobson Radical Unit Test","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Jacobson Radical Unit Test","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Jacobson Radical Unit Test

For $x$ in a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$,

$$
x\in J(A)
\iff
1-xy\text{ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Unit\|Unit]] for every }y\in A,
$$

where $J(A)$ is the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Jacobson Radical\|Jacobson Radical]].

## Proof

Suppose $x\in J(A)$ and $1-xy$ is not a unit for some $y$. By the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Krull's Maximal Ideal Theorem\|Krull's Maximal Ideal Theorem]], the nonunit $1-xy$ belongs to a maximal ideal $\mathfrak m$. Since $x\in J(A)\subseteq\mathfrak m$, also $xy\in\mathfrak m$. Hence

$$
1=(1-xy)+xy\in\mathfrak m,
$$

contradicting that $\mathfrak m$ is proper.

Conversely, suppose $x\notin\mathfrak m$ for some maximal ideal $\mathfrak m$. Maximality gives

$$
\mathfrak m+(x)=A,
$$

so $u+xy=1$ for some $u\in\mathfrak m$ and $y\in A$. Then $1-xy=u\in\mathfrak m$, and therefore $1-xy$ is not a unit. This is the contrapositive of the reverse implication.

## Useful consequence

If $x\in J(A)$, then $1-x$ is a unit by taking $y=1$. Every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Nilpotent Element\|Nilpotent Element]] lies in $J(A)$, so this recovers the familiar finite geometric-series inverse for $1-x$.

## Source

- 01_05_nilradical_jacobson_radical.pdf, printed p. 6; Proposition 1.9.

