---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Group Actions/"}
---


# Group Actions

## Introduction

The concept of a group "acting" on a set is a powerful generalization of the idea that groups represent symmetries. It provides a framework for studying how group elements permute or transform other mathematical objects, leading to some of the most important theorems in the subject.

## Definition

### Formal Definition

A **(left) group action** of a group $G$ on a set $X$ is a map $G \times X \to X$, denoted by $(g, x) \mapsto g \cdot x$, that satisfies two axioms for all $g, h \in G$ and $x \in X$:

1. **Identity**: $e \cdot x = x$
2. **Compatibility**: $g \cdot (h \cdot x) = (gh) \cdot x$

### Alternative Definition

Equivalently, a group action is a homomorphism $\phi: G \to \text{Sym}(X)$, where $\text{Sym}(X)$ is the group of all permutations of the set $X$. The kernel of this homomorphism, $\ker(\phi) = \{g \in G \mid g \cdot x = x \text{ for all } x \in X\}$, consists of the elements of $G$ that act trivially on $X$.

## Properties of Actions

### Faithful Actions
The action is **faithful** if the kernel is trivial ($\ker(\phi) = \{e\}$). In this case, $G$ is isomorphic to a subgroup of $\text{Sym}(X)$.

### Transitive Actions
The action is **transitive** if for any two elements $x, y \in X$, there exists a $g \in G$ such that $g \cdot x = y$. This means the group can move any element to any other element.

### Free Actions
The action is **free** if the stabilizer of every element is trivial, i.e., $g \cdot x = x$ implies $g = e$.

### Regular Actions
The action is **regular** if it is both transitive and free.

## Examples

### Example 1: Natural Action of $S_n$

The symmetric group $S_n$ acts on the set $\{1, 2, \ldots, n\}$. This is the **natural action**:
- For $\sigma \in S_n$ and $i \in \{1, 2, \ldots, n\}$, we define $\sigma \cdot i = \sigma(i)$
- This action is faithful and transitive

### Example 2: Dihedral Group Action

The dihedral group $D_n$ acts on the set of vertices of a regular $n$-gon:
- Rotations and reflections permute the vertices
- This action is faithful and transitive

### Example 3: Left Multiplication Action

Any group $G$ acts on itself by left multiplication: $(g, x) \mapsto gx$. This action is always faithful and regular (transitive and free).

### Example 4: Conjugation Action

Any group $G$ acts on itself by conjugation: $(g, x) \mapsto gxg^{-1}$. This action is fundamental for studying the internal structure of the group.

### Example 5: Action on Cosets

Let $H$ be a subgroup of $G$. Then $G$ acts on the set of left cosets $G/H$ by left multiplication: $(g, aH) \mapsto gaH$.

## Applications

### Application 1: Cayley's Theorem

The left multiplication action of a group on itself provides a proof of Cayley's theorem: every group is isomorphic to a subgroup of a symmetric group.

### Application 2: Understanding Group Structure

Group actions help us understand the structure of groups by studying how they act on various sets.

### Application 3: Combinatorics

Group actions are fundamental in combinatorics, particularly in counting problems involving symmetry.

### Application 4: Geometry

Group actions are essential in geometry, where they represent symmetries of geometric objects.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbits\|Orbits]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Stabilizers\|Stabilizers]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbit-Stabilizer Theorem\|Orbit-Stabilizer Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Semi-direct Products\|Semi-direct Products]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Group Homomorphisms\|Group Homomorphisms]] 