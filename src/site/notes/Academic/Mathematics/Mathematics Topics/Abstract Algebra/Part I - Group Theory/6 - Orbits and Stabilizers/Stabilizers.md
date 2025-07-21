---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Stabilizers/"}
---


# Stabilizers

## Introduction

When a group acts on a set, the stabilizer of an element consists of all group elements that fix that element. Stabilizers are fundamental to understanding group actions and provide crucial information about the group's structure.

## Definition

**Definition 6.1**: Let a group $G$ act on a set $X$. The **stabilizer** of an element $x \in X$ is the set of all elements in $G$ that fix $x$. It is a subgroup of $G$, denoted $\text{Stab}_G(x)$ or $G_x$:

$$\text{Stab}_G(x) = \{g \in G \mid g \cdot x = x\}$$

## Key Properties

### Subgroup Property
The stabilizer of any element is a subgroup of $G$. This follows from:
- **Closure**: If $g, h \in \text{Stab}_G(x)$, then $(gh) \cdot x = g \cdot (h \cdot x) = g \cdot x = x$
- **Identity**: $e \cdot x = x$, so $e \in \text{Stab}_G(x)$
- **Inverses**: If $g \in \text{Stab}_G(x)$, then $g^{-1} \cdot x = g^{-1} \cdot (g \cdot x) = (g^{-1}g) \cdot x = e \cdot x = x$

### Relationship to Orbits
Stabilizers are fundamentally linked to orbits through the Orbit-Stabilizer Theorem.

## Examples

### Example 1: Natural Action of $S_3$

Consider the natural action of $S_3$ on $\{1, 2, 3\}$:
- The stabilizer of 1 is $\text{Stab}_{S_3}(1) = \{e, (2,3)\}$
- The stabilizer of 2 is $\text{Stab}_{S_3}(2) = \{e, (1,3)\}$
- The stabilizer of 3 is $\text{Stab}_{S_3}(3) = \{e, (1,2)\}$

### Example 2: Action of $D_4$ on Vertices

Consider the action of $D_4$ on the vertices of a square:
- The stabilizer of a vertex consists of the identity and the reflection across the diagonal through that vertex
- $\text{Stab}_{D_4}(v) = \{e, \text{reflection through } v\}$

### Example 3: Conjugation Action

When a group $G$ acts on itself by conjugation:
- The stabilizer of an element $x$ is its **centralizer**: $C_G(x) = \{g \in G \mid gx = xg\}$
- Elements in the centralizer commute with $x$

### Example 4: Left Multiplication Action

When a group $G$ acts on itself by left multiplication:
- The stabilizer of any element is trivial: $\text{Stab}_G(x) = \{e\}$
- This is why the action is free

## Applications

### Application 1: Understanding Group Structure
Stabilizers help us understand the internal structure of groups by revealing which elements fix particular points.

### Application 2: Orbit-Stabilizer Theorem
Stabilizers are essential for the Orbit-Stabilizer Theorem, which relates orbit size to stabilizer index.

### Application 3: Class Equation
When studying conjugation actions, stabilizers (centralizers) lead to the Class Equation.

### Application 4: Counting Problems
Stabilizers are crucial in counting problems involving symmetry, particularly in combinatorics.

## Special Cases

### Trivial Stabilizer
If $\text{Stab}_G(x) = \{e\}$ for all $x \in X$, the action is called **free**.

### Full Stabilizer
If $\text{Stab}_G(x) = G$ for some $x \in X$, then $x$ is a **fixed point** of the action.

### Normal Subgroup
If $N$ is a normal subgroup of $G$, then $N$ is the stabilizer of the identity coset in the action of $G$ on $G/N$.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbits\|Orbits]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbit-Stabilizer Theorem\|Orbit-Stabilizer Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Group Actions\|Group Actions]]
- [[Centralizers\|Centralizers]]
- [[Conjugacy Classes\|Conjugacy Classes]] 