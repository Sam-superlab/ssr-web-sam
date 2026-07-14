---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal/","title":"Ideal","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Ideal","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Ideal

An **ideal** $\mathfrak a$ of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ is an additive subgroup $\mathfrak a\subseteq A$ such that

$$
A\mathfrak a\subseteq\mathfrak a.
$$

Equivalently:

- $0\in\mathfrak a$;
- $x-y\in\mathfrak a$ whenever $x,y\in\mathfrak a$;
- $ax\in\mathfrak a$ whenever $a\in A$ and $x\in\mathfrak a$.

The absorption condition distinguishes ideals from arbitrary [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Subring\|subrings]].

## Extremal ideals

Every ring has the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Zero Ideal\|Zero Ideal]] $(0)$ and the **unit ideal** $(1)=A$. An ideal is **proper** when $\mathfrak a\neq A$. Because $1\in\mathfrak a$ forces $A=A1\subseteq\mathfrak a$, an ideal is proper exactly when it does not contain $1$.

## Examples and nonexamples

- $n\mathbb Z$ is an ideal of $\mathbb Z$.
- $(x,y)\subseteq k[x,y]$ consists of polynomials with zero constant term.
- $\mathbb Z\subseteq\mathbb Q$ is a subring but not an ideal.
- The union of two ideals need not be an ideal: $(2)\cup(3)\subseteq\mathbb Z$ contains $2$ and $3$ but not $5$.

## Why ideals are the correct quotients

For $x+\mathfrak a=x'+\mathfrak a$ and $y+\mathfrak a=y'+\mathfrak a$, ideal absorption ensures $xy-x'y'\in\mathfrak a$. Hence multiplication descends to the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Quotient Ring\|Quotient Ring]] $A/\mathfrak a$.

Important special ideals include [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Principal Ideal\|principal]], [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|prime]], and [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Maximal Ideal\|maximal ideals]].

## Source

- 01_02_ideals_quotient_rings.pdf, printed p. 2 (definition of ideal).

