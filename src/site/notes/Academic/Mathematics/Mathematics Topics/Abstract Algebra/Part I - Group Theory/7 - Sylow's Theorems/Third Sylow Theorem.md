---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/Third Sylow Theorem/"}
---


# Third Sylow Theorem

## Introduction

The Third Sylow Theorem provides detailed information about the number of Sylow $p$-subgroups in a finite group. It gives precise constraints on this number, making it a powerful tool for group classification.

## Statement

**Third Sylow Theorem (Number)**: Let $n_p$ be the number of Sylow $p$-subgroups of $G$. Then:
- $n_p$ divides $m$ (the part of the group order not divisible by $p$)
- $n_p \equiv 1 \pmod{p}$
- $n_p = [G : N_G(P)]$, where $P$ is any Sylow $p$-subgroup and $N_G(P)$ is its normalizer in $G$

Let $G$ be a finite group of order $|G| = p^n m$, where $p$ is a prime and $p$ does not divide $m$.

## Proof Sketch

The proof uses group actions:

1. **Define the action**: Let $G$ act on the set of all its Sylow $p$-subgroups by conjugation.

2. **Transitivity**: By the Second Sylow Theorem, this action is transitive, so there is only one orbit.

3. **Count the orbit**: The size of this orbit is $n_p$.

4. **Modular constraint**: Restrict the action to a single Sylow $p$-subgroup $P$ and count fixed points to get $n_p \equiv 1 \pmod{p}$.

### Key Steps

- The action of $G$ on the set of Sylow $p$-subgroups is transitive
- The size of the orbit is $n_p = [G : N_G(P)]$
- When $P$ acts on the set of Sylow $p$-subgroups, it fixes itself and possibly others
- The number of fixed points is congruent to $n_p$ modulo $p$

## Examples

### Example 1: Groups of Order 12

Let $G$ be a group of order 12. We have $12 = 2^2 \cdot 3$.

**Sylow 2-subgroups**: $n_2$ must divide 3 and $n_2 \equiv 1 \pmod{2}$. So $n_2 = 1$ or $n_2 = 3$.

**Sylow 3-subgroups**: $n_3$ must divide 4 and $n_3 \equiv 1 \pmod{3}$. So $n_3 = 1$ or $n_3 = 4$.

### Example 2: Groups of Order 30

Let $G$ be a group of order 30. We have $30 = 2 \cdot 3 \cdot 5$.

**Sylow 2-subgroups**: $n_2$ must divide 15 and $n_2 \equiv 1 \pmod{2}$. So $n_2 = 1, 3, 5, 15$.

**Sylow 3-subgroups**: $n_3$ must divide 10 and $n_3 \equiv 1 \pmod{3}$. So $n_3 = 1$ or $n_3 = 10$.

**Sylow 5-subgroups**: $n_5$ must divide 6 and $n_5 \equiv 1 \pmod{5}$. So $n_5 = 1$ or $n_5 = 6$.

### Example 3: Groups of Order 15

A group of order 15 must have $n_3 = 1$ and $n_5 = 1$. The unique Sylow 3-subgroup and Sylow 5-subgroup are both normal, and it can be shown that the group must be the cyclic group $\mathbb{Z}_{15}$.

## Applications

### Application 1: Group Classification

The Third Sylow Theorem is crucial for classifying groups of a given order by constraining the number of Sylow subgroups.

### Application 2: Simplicity Tests

If $n_p = 1$ for some prime $p$, the unique Sylow $p$-subgroup is normal, so the group is not simple.

### Application 3: Structure Analysis

The constraints on $n_p$ help determine the possible structure of finite groups.

## Consequences

### Divisibility Constraints

The theorem provides strong constraints on the number of Sylow subgroups, which are essential for group classification.

### Normalizer Information

The relationship $n_p = [G : N_G(P)]$ connects the number of Sylow subgroups to the structure of normalizers.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/First Sylow Theorem\|First Sylow Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/Second Sylow Theorem\|Second Sylow Theorem]]
- [[Sylow Subgroups\|Sylow Subgroups]]
- [[Normalizers\|Normalizers]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Group Actions\|Group Actions]] 