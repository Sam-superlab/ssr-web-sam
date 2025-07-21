---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/Second Sylow Theorem/"}
---


# Second Sylow Theorem

## Introduction

The Second Sylow Theorem establishes that all Sylow $p$-subgroups of a finite group are conjugate to one another. This is a powerful result that shows the uniqueness of Sylow subgroups up to conjugation.

## Statement

**Second Sylow Theorem (Conjugacy)**: All Sylow $p$-subgroups of $G$ are conjugate to one another. That is, if $P_1$ and $P_2$ are Sylow $p$-subgroups, then there exists a $g \in G$ such that $P_1 = gP_2g^{-1}$. This also implies that any $p$-subgroup is contained within some Sylow $p$-subgroup.

Let $G$ be a finite group of order $|G| = p^n m$, where $p$ is a prime and $p$ does not divide $m$.

## Proof Sketch

The proof uses group actions:

1. **Define the action**: Let a Sylow $p$-subgroup $P$ act on the set of left cosets of another Sylow $p$-subgroup $Q$.

2. **Apply orbit-stabilizer**: Show that there must be a fixed point under this action.

3. **Conclude conjugacy**: The existence of a fixed point implies that $P$ is a conjugate of $Q$.

### Key Steps

- The action of $P$ on $G/Q$ has orbits of size dividing $|P| = p^n$
- Since $[G:Q] = m$ is not divisible by $p$, there must be a fixed point
- A fixed point corresponds to $gQ$ where $P \subseteq gQg^{-1}$
- Since both have the same order, $P = gQg^{-1}$

## Examples

### Example 1: Groups of Order 12

Let $G$ be a group of order 12. We have $12 = 2^2 \cdot 3$.

- All Sylow 2-subgroups (order 4) are conjugate
- All Sylow 3-subgroups (order 3) are conjugate

### Example 2: Groups of Order 30

Let $G$ be a group of order 30. We have $30 = 2 \cdot 3 \cdot 5$.

- All Sylow 2-subgroups (order 2) are conjugate
- All Sylow 3-subgroups (order 3) are conjugate
- All Sylow 5-subgroups (order 5) are conjugate

### Example 3: Symmetric Groups

In $S_4$ (order 24):
- All Sylow 2-subgroups (order 8) are conjugate
- All Sylow 3-subgroups (order 3) are conjugate

## Applications

### Application 1: Normal Sylow Subgroups

If a group has a unique Sylow $p$-subgroup (i.e., $n_p = 1$), then that subgroup is normal, since it is its only conjugate.

### Application 2: Group Classification

The Second Sylow Theorem helps classify groups by understanding the conjugacy of their Sylow subgroups.

### Application 3: Simplicity Tests

If a group has multiple Sylow $p$-subgroups, they must be conjugate, which can help determine if the group is simple.

## Consequences

### Uniqueness Up to Conjugation

The theorem shows that Sylow $p$-subgroups are unique up to conjugation, providing a strong structural result.

### Containment of p-Subgroups

Any $p$-subgroup is contained within some Sylow $p$-subgroup, giving a complete picture of $p$-subgroup structure.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/First Sylow Theorem\|First Sylow Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/Third Sylow Theorem\|Third Sylow Theorem]]
- [[Sylow Subgroups\|Sylow Subgroups]]
- [[Conjugacy\|Conjugacy]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]] 