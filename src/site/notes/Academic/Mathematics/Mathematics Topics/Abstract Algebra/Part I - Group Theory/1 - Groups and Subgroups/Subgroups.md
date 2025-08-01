---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Subgroups/"}
---


# Subgroups

## Introduction

Within a group, there often exist smaller groups. A **subgroup** is a subset of a group that itself forms a group under the same operation.

## Definition

A **subgroup** $H$ of a group $G$ is a non-empty subset of $G$ that itself forms a group under the binary operation of $G$. This is denoted by $H \leq G$.

### Types of Subgroups

- If $H$ is a proper subset of $G$ ($H \neq G$), it is a **proper subgroup**, denoted $H < G$
- The subgroup $\{e\}$ consisting of only the identity element is the **trivial subgroup**
- The group $G$ itself is always a subgroup of $G$

## Subgroup Tests

To verify that a non-empty subset $H \subseteq G$ is a subgroup, one can use the following tests:

### Two-Step Test
$H$ is a subgroup if and only if:
1. It is closed under the group operation (for all $a, b \in H$, $ab \in H$)
2. It is closed under inverses (for all $a \in H$, $a^{-1} \in H$)

### One-Step Test
$H$ is a subgroup if and only if for all $a, b \in H$, the element $ab^{-1}$ is also in $H$.

### Finite Subgroup Test
If $H$ is a finite, non-empty subset of $G$, it is a subgroup if and only if it is closed under the group operation.

## Examples

### Example 1: Subgroups of $(\mathbb{Z}, +)$
- The set of even integers $2\mathbb{Z} = \{0, \pm2, \pm4, \ldots\}$ is a subgroup
- For any $n \in \mathbb{N}$, the set $n\mathbb{Z} = \{0, \pm n, \pm 2n, \ldots\}$ is a subgroup
- The set $\{0\}$ is the trivial subgroup

### Example 2: Subgroups of $D_4$
- The set of rotations $\{e, r, r^2, r^3\}$ is a subgroup
- The set $\{e, r^2\}$ is a subgroup (rotations by $0°$ and $180°$)
- The set $\{e, s\}$ is a subgroup (identity and horizontal reflection)
- The set $\{e, sr^2\}$ is a subgroup (identity and diagonal reflection)

### Example 3: Subgroups of $S_3$
- The alternating group $A_3 = \{e, (1,2,3), (1,3,2)\}$ is a subgroup
- Any cyclic subgroup generated by a single element, e.g., $\langle (1,2) \rangle = \{e, (1,2)\}$
- The trivial subgroup $\{e\}$

### Example 4: Subgroups of $(\mathbb{R}^*, \cdot)$
- The positive real numbers $\mathbb{R}^+$ form a subgroup
- The set $\{1, -1\}$ forms a subgroup
- The set $\{1\}$ is the trivial subgroup

## Properties of Subgroups

### Intersection of Subgroups
The intersection of any collection of subgroups of $G$ is itself a subgroup of $G$.

### Subgroup Generated by a Set
For any subset $S \subseteq G$, the **subgroup generated by $S$**, denoted $\langle S \rangle$, is the smallest subgroup of $G$ containing $S$.

### Cyclic Subgroups
If $S = \{a\}$ is a singleton, then $\langle a \rangle = \{a^n \mid n \in \mathbb{Z}\}$ is called the **cyclic subgroup generated by $a$**.

## Lagrange's Theorem

**Theorem**: If $G$ is a finite group and $H$ is a subgroup of $G$, then the order of $H$ divides the order of $G$.

This theorem places a strong restriction on the possible sizes of subgroups.

## Examples of Subgroup Calculations

### Example 1: Finding All Subgroups of $\mathbb{Z}_{12}$
The subgroups of $\mathbb{Z}_{12}$ are:
- $\{0\}$ (order 1)
- $\{0, 6\}$ (order 2)
- $\{0, 4, 8\}$ (order 3)
- $\{0, 3, 6, 9\}$ (order 4)
- $\{0, 2, 4, 6, 8, 10\}$ (order 6)
- $\mathbb{Z}_{12}$ itself (order 12)

### Example 2: Subgroups of $D_6$
The dihedral group $D_6$ has order 12. Its subgroups include:
- $\{e\}$ (order 1)
- $\{e, r^3\}$ (order 2)
- $\{e, r^2, r^4\}$ (order 3)
- $\{e, r^3, s, sr^3\}$ (order 4)
- $\{e, r, r^2, r^3, r^4, r^5\}$ (order 6)
- $D_6$ itself (order 12)

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Group Axioms\|Group Axioms]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Cosets\|Cosets]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Quotient Groups\|Quotient Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Lagrange's Theorem\|Lagrange's Theorem]] 