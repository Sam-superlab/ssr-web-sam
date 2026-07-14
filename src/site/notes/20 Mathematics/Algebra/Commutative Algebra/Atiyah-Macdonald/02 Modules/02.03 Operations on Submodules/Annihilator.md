---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.03 Operations on Submodules/Annihilator/","dg-note-properties":{}}
---


# Annihilator

The **annihilator** of an $A$-module $M$ is

$$\operatorname{Ann}_A(M)=\{a\in A:aM=0\}=(0:M).$$

It is an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Ideal\|Ideal]] and is precisely the kernel of the action map $A\to\operatorname{End}_{\mathbb Z}(M)$. Thus it measures how much of the scalar ring acts invisibly.

If $\mathfrak a\subseteq\operatorname{Ann}_A(M)$, the action factors through the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Quotient Ring\|Quotient Ring]] $A/\mathfrak a$. In particular, every $M$ is a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.03 Operations on Submodules/Faithful Module\|Faithful Module]] over $A/\operatorname{Ann}_A(M)$.

## Examples

- $\operatorname{Ann}_A(A/I)=I$.
- $\operatorname{Ann}_{\mathbb Z}(\mathbb Z/n\mathbb Z)=n\mathbb Z$.
- $\operatorname{Ann}_A(A)=0$.

Exercise 2.2 gives $\operatorname{Ann}(M\oplus N)=\operatorname{Ann}(M)\cap\operatorname{Ann}(N)$.

## Source

- `02_03_operations_on_submodules.pdf`, printed pp. 19-20; Exercise 2.2.
