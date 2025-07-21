---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/Sylow's Theorems/"}
---


# Sylow's Theorems

## Introduction

Lagrange's Theorem states that the order of a subgroup must divide the order of the group. However, it does not guarantee the existence of a subgroup for every divisor of the group's order. The Sylow theorems, named after the Norwegian mathematician Peter Ludwig Sylow, provide a powerful partial converse, guaranteeing the existence of subgroups of prime-power order and providing detailed information about their number and properties. These theorems are the primary tools for analyzing the structure of finite groups.

## Statement of the Sylow Theorems

Let $G$ be a finite group of order $|G| = p^n m$, where $p$ is a prime and $p$ does not divide $m$. A subgroup of order $p^n$ is called a **Sylow $p$-subgroup** of $G$.

**Theorem 7.1 (The Sylow Theorems)**:

1. **First Sylow Theorem (Existence)**: For any prime factor $p$ of $|G|$, Sylow $p$-subgroups of $G$ exist.

2. **Second Sylow Theorem (Conjugacy)**: All Sylow $p$-subgroups of $G$ are conjugate to one another. That is, if $P_1$ and $P_2$ are Sylow $p$-subgroups, then there exists a $g \in G$ such that $P_1 = gP_2g^{-1}$. This also implies that any $p$-subgroup is contained within some Sylow $p$-subgroup.

3. **Third Sylow Theorem (Number)**: Let $n_p$ be the number of Sylow $p$-subgroups of $G$. Then:
   - $n_p$ divides $m$ (the part of the group order not divisible by $p$)
   - $n_p \equiv 1 \pmod{p}$
   - $n_p = [G : N_G(P)]$, where $P$ is any Sylow $p$-subgroup and $N_G(P)$ is its normalizer in $G$

## Proof Sketch

The proofs of the Sylow theorems are elegant applications of group actions.

### First Theorem

Let $G$ act on the set of all subsets of size $p^n$. A combinatorial argument shows that there must be an orbit whose size is not divisible by $p$. The stabilizer of any element in this orbit is a subgroup of order $p^n$.

### Second Theorem

Let a Sylow $p$-subgroup $P$ act on the set of left cosets of another Sylow $p$-subgroup $Q$. An application of the orbit-stabilizer theorem shows there must be a fixed point, which implies $P$ is a conjugate of $Q$.

### Third Theorem

Let $G$ act on the set of all its Sylow $p$-subgroups by conjugation. By the second theorem, this action is transitive, so there is only one orbit. The size of this orbit is $n_p$. The result $n_p \equiv 1 \pmod{p}$ is obtained by restricting this action to a single Sylow $p$-subgroup $P$ and counting the fixed points.

## Applications

The Sylow theorems are incredibly useful for determining the structure of a finite group. For example, if $n_p = 1$ for some prime $p$, the unique Sylow $p$-subgroup must be normal (since it is its only conjugate). This is often the first step in proving that a group of a certain order cannot be simple.

### Example: Groups of Order 15

A group of order 15 must have $n_3 = 1$ and $n_5 = 1$. The unique Sylow 3-subgroup and Sylow 5-subgroup are both normal, and it can be shown that the group must be the cyclic group $\mathbb{Z}_{15}$.

## Summary

The Sylow theorems provide powerful tools for understanding the structure of finite groups. They guarantee the existence of subgroups of prime-power order and provide detailed information about their number and properties. These theorems are fundamental to finite group theory and have applications throughout mathematics.

The Sylow theorems are particularly useful for:
- Determining the structure of groups of small order
- Proving that certain groups are not simple
- Understanding the relationship between different subgroups
- Classifying finite groups up to isomorphism

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/First Sylow Theorem\|First Sylow Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/Second Sylow Theorem\|Second Sylow Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/7 - Sylow's Theorems/Third Sylow Theorem\|Third Sylow Theorem]]
- [[Sylow Subgroups\|Sylow Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Group Actions\|Group Actions]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbit-Stabilizer Theorem\|Orbit-Stabilizer Theorem]] 