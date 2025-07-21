---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/8 - Commutator Subgroups/Nilpotent Groups/"}
---


# Nilpotent Groups

## Introduction

Nilpotent groups are a special subclass of solvable groups that are "almost abelian." They have a more constrained structure than solvable groups, making them closer to abelian groups.

## Definition

**Definition 8.4**: A group $G$ is **nilpotent** if its upper central series terminates at $G$. The upper central series is defined recursively: $Z_0(G) = \{e\}$, and $Z_{i+1}(G)$ is the subgroup of $G$ such that $Z_{i+1}(G)/Z_i(G) = Z(G/Z_i(G))$.

Alternatively, a group is nilpotent if its lower central series terminates at $\{e\}$, where $\gamma_1(G) = G$ and $\gamma_{i+1}(G) = [G, \gamma_i(G)]$.

## Properties

- All nilpotent groups are solvable, but the converse is not true ($S_3$ is solvable but not nilpotent)
- All finite $p$-groups are nilpotent
- A key property of finite nilpotent groups is that they are the direct product of their Sylow subgroups

Nilpotent groups have a more constrained structure than solvable groups, making them closer to abelian groups. For example, in a finite nilpotent group, any two elements with relatively prime orders must commute.

## Examples

### Example 1: Abelian Groups

All abelian groups are both solvable and nilpotent. For an abelian group $G$, we have $G' = \{e\}$, so the derived series terminates immediately.

### Example 2: p-Groups

All finite $p$-groups are nilpotent. For example, the quaternion group $Q_8$ is nilpotent:
- $Z_0(Q_8) = \{e\}$
- $Z_1(Q_8) = \langle -1 \rangle$
- $Z_2(Q_8) = Q_8$

### Example 3: Direct Products

The direct product of nilpotent groups is nilpotent.

### Example 4: Non-Nilpotent Solvable Groups

The symmetric group $S_3$ is solvable but not nilpotent:
- $S_3' = A_3$
- $S_3'' = \{e\}$
- But the upper central series never reaches $S_3$

## Applications

### Application 1: Group Classification

Nilpotent groups are important in the classification of finite groups. Many important families of groups (such as $p$-groups) are nilpotent, and understanding their structure is crucial for the classification of all finite groups.

### Application 2: Representation Theory

Nilpotent groups have particularly nice properties in representation theory. For example, all irreducible representations of a finite nilpotent group are monomial (induced from one-dimensional representations of subgroups).

### Application 3: Structure Analysis

The constrained structure of nilpotent groups makes them easier to analyze than general solvable groups.

## Supersolvable Groups

A group $G$ is **supersolvable** if it has a normal series with cyclic factors. Supersolvable groups are a subclass of solvable groups that are even more constrained than nilpotent groups.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/8 - Commutator Subgroups/Commutator Subgroups\|Commutator Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/8 - Commutator Subgroups/Solvable Groups\|Solvable Groups]]
- [[p-Groups\|p-Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/4 - Jordan-Hölder Theorem/Direct Products\|Direct Products]]
- [[Central Series\|Central Series]] 