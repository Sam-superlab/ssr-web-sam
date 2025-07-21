---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbit-Stabilizer Theorem/"}
---


# Orbit-Stabilizer Theorem

## Introduction

The Orbit-Stabilizer Theorem is one of the most useful theorems in group theory. It provides a fundamental relationship between the size of orbits and the index of stabilizers, offering a powerful tool for counting and understanding group actions.

## Statement

**Theorem 6.2 (Orbit-Stabilizer Theorem)**: Let a finite group $G$ act on a set $X$. For any $x \in X$, the size of the orbit of $x$ is equal to the index of its stabilizer subgroup:

$$|\text{Orb}_G(x)| = \frac{|G|}{|\text{Stab}_G(x)|}$$

This theorem provides a powerful formula: $|G| = |\text{Orb}_G(x)| \cdot |\text{Stab}_G(x)|$.

## Proof Sketch

The proof uses the fact that there is a bijection between the orbit of $x$ and the set of left cosets of the stabilizer of $x$. Specifically, the map $g \cdot x \mapsto g\text{Stab}_G(x)$ is a well-defined bijection.

### Key Steps in the Proof

1. **Define the map**: $\phi: \text{Orb}_G(x) \to G/\text{Stab}_G(x)$ by $\phi(g \cdot x) = g\text{Stab}_G(x)$

2. **Show it's well-defined**: If $g_1 \cdot x = g_2 \cdot x$, then $g_1^{-1}g_2 \in \text{Stab}_G(x)$, so $g_1\text{Stab}_G(x) = g_2\text{Stab}_G(x)$

3. **Show it's injective**: If $\phi(g_1 \cdot x) = \phi(g_2 \cdot x)$, then $g_1 \cdot x = g_2 \cdot x$

4. **Show it's surjective**: Every coset $g\text{Stab}_G(x)$ is the image of $g \cdot x$

5. **Conclude**: Since there's a bijection, $|\text{Orb}_G(x)| = [G : \text{Stab}_G(x)] = |G|/|\text{Stab}_G(x)|$

## Examples

### Example 1: Action of $S_3$ on $\{1, 2, 3\}$

Consider the natural action of $S_3$ on $\{1, 2, 3\}$:
- The orbit of any element is the entire set $\{1, 2, 3\}$ (the action is transitive)
- The stabilizer of 1 is $\{e, (2,3)\}$
- By the orbit-stabilizer theorem: $|S_3| = 6 = 3 \cdot 2 = |\text{Orb}(1)| \cdot |\text{Stab}(1)|$

### Example 2: Action of $D_4$ on Vertices

Consider the action of $D_4$ on the vertices of a square:
- The orbit of any vertex is the entire set of vertices (transitive action)
- The stabilizer of a vertex consists of the identity and the reflection across the diagonal through that vertex
- By the orbit-stabilizer theorem: $|D_4| = 8 = 4 \cdot 2 = |\text{Orb}(v)| \cdot |\text{Stab}(v)|$

### Example 3: Conjugation Action

When a group $G$ acts on itself by conjugation:
- The orbit of an element $x$ is its **conjugacy class**: $\text{cl}(x) = \{gxg^{-1} \mid g \in G\}$
- The stabilizer of $x$ is its **centralizer**: $C_G(x) = \{g \in G \mid gx = xg\}$
- The orbit-stabilizer theorem gives: $|\text{cl}(x)| = [G : C_G(x)]$

## Applications

### Application 1: Counting Orbits

The orbit-stabilizer theorem is often used to count the number of elements in orbits, which is useful in combinatorics and group theory.

### Application 2: Understanding Group Structure

The theorem helps us understand the structure of groups by relating orbit sizes to subgroup indices.

### Application 3: Class Equation

When a group acts on itself by conjugation, the orbit-stabilizer theorem leads to the class equation, which is fundamental for understanding the structure of finite groups.

### Application 4: Burnside's Lemma

The orbit-stabilizer theorem is used in the proof of Burnside's Lemma, which counts the number of orbits.

## Special Cases

### Transitive Actions
If the action is transitive, then $|\text{Orb}_G(x)| = |X|$ for all $x \in X$, so $|G| = |X| \cdot |\text{Stab}_G(x)|$.

### Free Actions
If the action is free, then $|\text{Stab}_G(x)| = 1$ for all $x \in X$, so $|\text{Orb}_G(x)| = |G|$.

### Regular Actions
If the action is regular (transitive and free), then $|G| = |X|$.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbits\|Orbits]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Stabilizers\|Stabilizers]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Group Actions\|Group Actions]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Class Equation\|Class Equation]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Burnside's Lemma\|Burnside's Lemma]] 