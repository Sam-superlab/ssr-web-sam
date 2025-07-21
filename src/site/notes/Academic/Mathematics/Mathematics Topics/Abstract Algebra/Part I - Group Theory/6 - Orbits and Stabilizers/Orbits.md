---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbits/"}
---


# Orbits

## Introduction

When a group acts on a set, it partitions the set into disjoint pieces called orbits. Understanding orbits is fundamental to understanding group actions and their applications.

## Definition

**Definition 6.1**: Let a group $G$ act on a set $X$. The **orbit** of an element $x \in X$ is the set of all elements in $X$ that $x$ can be moved to by the action of $G$. It is denoted $\text{Orb}_G(x)$ or $G \cdot x$:

$$\text{Orb}_G(x) = \{g \cdot x \mid g \in G\}$$

## Key Properties

### Partition Property
The orbits form a partition of the set $X$. This means that:
- Every element of $X$ belongs to exactly one orbit
- Any two orbits are either identical or disjoint

### Equivalence Relation
The relation $x \sim y$ if and only if $y \in \text{Orb}_G(x)$ is an equivalence relation on $X$, and the equivalence classes are precisely the orbits.

### Transitive Actions
If the action is transitive, there is only one orbit: the entire set $X$.

## Examples

### Example 1: Natural Action of $S_3$

Consider the natural action of $S_3$ on $\{1, 2, 3\}$:
- The orbit of any element is the entire set $\{1, 2, 3\}$ (the action is transitive)
- $\text{Orb}_{S_3}(1) = \text{Orb}_{S_3}(2) = \text{Orb}_{S_3}(3) = \{1, 2, 3\}$

### Example 2: Action of $D_4$ on Vertices

Consider the action of $D_4$ on the vertices of a square:
- The orbit of any vertex is the entire set of vertices (transitive action)
- $\text{Orb}_{D_4}(v) = \{\text{all vertices}\}$ for any vertex $v$

### Example 3: Conjugation Action

When a group $G$ acts on itself by conjugation:
- The orbit of an element $x$ is its **conjugacy class**: $\text{cl}(x) = \{gxg^{-1} \mid g \in G\}$
- Different elements may have different sized orbits

### Example 4: Action on Cosets

Let $H$ be a subgroup of $G$. When $G$ acts on the set of left cosets $G/H$ by left multiplication:
- The orbit of any coset is the entire set $G/H$ (transitive action)

## Applications

### Application 1: Understanding Group Structure
Orbits help us understand how a group acts on a set and reveal information about the group's structure.

### Application 2: Counting Problems
Orbits are fundamental in counting problems involving symmetry, particularly in combinatorics.

### Application 3: Geometry
Orbits represent the "paths" that elements can follow under the group action, which is important in geometry and symmetry.

### Application 4: Representation Theory
Orbits are important in representation theory, where they correspond to irreducible representations.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Stabilizers\|Stabilizers]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbit-Stabilizer Theorem\|Orbit-Stabilizer Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Group Actions\|Group Actions]]
- [[Conjugacy Classes\|Conjugacy Classes]]
- [[Transitive Actions\|Transitive Actions]] 