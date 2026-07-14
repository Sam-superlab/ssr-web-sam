---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Colon Ideal of Submodules/","title":"Colon Ideal of Submodules","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"],"dg-note-properties":{"title":"Colon Ideal of Submodules","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"]}}
---


# Colon Ideal of Submodules

For submodules $N,P\subseteq M$, the **colon ideal** is

$$(N:P)=\{a\in A:aP\subseteq N\}.$$

It is an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] of $A$. It measures which scalars force all of $P$ into $N$.

Special cases clarify the meaning:

- $(0:M)=\operatorname{Ann}_A(M)$ is the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Foundations/Annihilator\|Annihilator]].
- $(N:M)$ consists of scalars that make all of $M$ vanish in $M/N$.
- Exercise 2.2 identifies $(N:P)$ with the annihilator of $(N+P)/N$.

This notation generalizes the ideal quotient from Chapter 1 while allowing the compared objects to be submodules.

## Source

- `02_03_operations_on_submodules.pdf`, printed pp. 19-20; Exercise 2.2(ii).
