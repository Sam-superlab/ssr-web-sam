---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/First Sylow Theorem/"}
---


# First Sylow Theorem

## Introduction

The First Sylow Theorem guarantees the existence of Sylow $p$-subgroups for any prime factor $p$ of a finite group's order. This is a powerful existence result that provides a partial converse to Lagrange's Theorem.

## Statement

**First Sylow Theorem (Existence)**: For any prime factor $p$ of $|G|$, Sylow $p$-subgroups of $G$ exist.

Let $G$ be a finite group of order $|G| = p^n m$, where $p$ is a prime and $p$ does not divide $m$. A subgroup of order $p^n$ is called a **Sylow $p$-subgroup** of $G$.

## Proof Sketch

The proof is an elegant application of group actions:

1. **Define the action**: Let $G$ act on the set of all subsets of size $p^n$ by left multiplication.

2. **Combinatorial argument**: Show that there must be an orbit whose size is not divisible by $p$.

3. **Stabilizer is the subgroup**: The stabilizer of any element in this orbit is a subgroup of order $p^n$.

### Key Steps

- The number of subsets of size $p^n$ is $\binom{|G|}{p^n}$
- By Lucas's theorem or direct calculation, this number is not divisible by $p$
- Since the orbits partition the set, at least one orbit has size not divisible by $p$
- The stabilizer of any element in such an orbit has order $p^n$

## Examples

### Example 1: Groups of Order 12

Let $G$ be a group of order 12. We have $12 = 2^2 \cdot 3$.

- By the First Sylow Theorem, $G$ has Sylow 2-subgroups of order 4
- $G$ also has Sylow 3-subgroups of order 3

### Example 2: Groups of Order 30

Let $G$ be a group of order 30. We have $30 = 2 \cdot 3 \cdot 5$.

- By the First Sylow Theorem, $G$ has Sylow 2-subgroups of order 2
- $G$ has Sylow 3-subgroups of order 3
- $G$ has Sylow 5-subgroups of order 5

### Example 3: Symmetric Groups

In $S_4$ (order 24), the First Sylow Theorem guarantees:
- Sylow 2-subgroups of order 8
- Sylow 3-subgroups of order 3

## Applications

### Application 1: Group Classification

The First Sylow Theorem is the first step in classifying groups of a given order, as it guarantees the existence of certain subgroups.

### Application 2: Structure Analysis

Knowing that Sylow $p$-subgroups exist helps us understand the structure of finite groups.

### Application 3: Simplicity Tests

The existence of Sylow subgroups is crucial for testing whether a group is simple.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/Second Sylow Theorem\|Second Sylow Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/Third Sylow Theorem\|Third Sylow Theorem]]
- [[Sylow Subgroups\|Sylow Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Group Actions\|Group Actions]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Lagrange's Theorem\|Lagrange's Theorem]] 