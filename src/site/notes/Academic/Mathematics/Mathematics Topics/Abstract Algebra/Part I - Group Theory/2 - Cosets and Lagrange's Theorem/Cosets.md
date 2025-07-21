---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Cosets/"}
---


# Cosets

## Introduction

A subgroup $H$ of a group $G$ provides a natural way to partition the elements of $G$ into equal-sized pieces called cosets. This partitioning is fundamental to understanding the structure of groups.

## Definition

**Definition 2.1**: Let $H$ be a subgroup of a group $G$, and let $g \in G$.

- The **left coset** of $H$ with respect to $g$ is the set $gH = \{gh \mid h \in H\}$
- The **right coset** of $H$ with respect to $g$ is the set $Hg = \{hg \mid h \in H\}$
- The element $g$ is called a **coset representative**

## Key Properties of Cosets

### 1. Partition Property
The left cosets of $H$ in $G$ form a partition of the set $G$. This means that:
- Every element of $G$ belongs to exactly one left coset
- Any two left cosets are either identical or disjoint

### 2. Equivalence Relation
This can be proven formally by showing that the relation $a \sim b$ if and only if $a^{-1}b \in H$ is an equivalence relation on $G$, where the equivalence classes are precisely the left cosets of $H$.

### 3. Equal Cardinality
There is a simple bijection between any subgroup $H$ and any of its cosets $gH$ (given by the map $h \mapsto gh$). This implies that all cosets of $H$ have the same cardinality as $H$ itself.

## Examples

### Example 1: Cosets in $D_4$

Consider the dihedral group $D_4$ and the subgroup $H = \{e, r^2\}$ (rotations by $0°$ and $180°$):

- $eH = \{e \cdot e, e \cdot r^2\} = \{e, r^2\}$
- $rH = \{r \cdot e, r \cdot r^2\} = \{r, r^3\}$
- $sH = \{s \cdot e, s \cdot r^2\} = \{s, sr^2\}$
- $srH = \{sr \cdot e, sr \cdot r^2\} = \{sr, sr^3\}$

These four cosets partition $D_4$ into equal-sized pieces, each containing 2 elements.

### Example 2: Cosets in $(\mathbb{Z}, +)$

Consider the subgroup $H = 3\mathbb{Z} = \{0, \pm3, \pm6, \ldots\}$ in $(\mathbb{Z}, +)$:

- $0 + H = \{0, \pm3, \pm6, \ldots\} = H$
- $1 + H = \{1, 4, 7, \ldots, -2, -5, \ldots\}$
- $2 + H = \{2, 5, 8, \ldots, -1, -4, \ldots\}$

These three cosets partition $\mathbb{Z}$ into three infinite sets.

### Example 3: Cosets in $S_3$

Consider the subgroup $H = \{e, (1,2)\}$ in $S_3$:

- $eH = \{e, (1,2)\}$
- $(1,3)H = \{(1,3), (1,2,3)\}$
- $(2,3)H = \{(2,3), (1,3,2)\}$

These three cosets partition $S_3$ into equal-sized pieces.

## Properties

### Coset Representatives
Any element of a coset can serve as a coset representative. If $g' \in gH$, then $g'H = gH$.

### Left vs Right Cosets
In general, left cosets and right cosets may be different. However, they coincide if and only if the subgroup is normal.

### Number of Cosets
The number of left cosets equals the number of right cosets, and this number is called the **index** of $H$ in $G$, denoted $[G : H]$.

## Applications

### Application 1: Group Partitioning
Cosets provide a systematic way to partition a group into equal-sized pieces.

### Application 2: Index Calculations
The index $[G : H]$ can be calculated as $[G : H] = |G|/|H|$ for finite groups.

### Application 3: Normal Subgroups
The study of when left and right cosets coincide leads to the concept of normal subgroups.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Subgroups\|Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Lagrange's Theorem\|Lagrange's Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Quotient Groups\|Quotient Groups]]
- [[Index of a Subgroup\|Index of a Subgroup]] 