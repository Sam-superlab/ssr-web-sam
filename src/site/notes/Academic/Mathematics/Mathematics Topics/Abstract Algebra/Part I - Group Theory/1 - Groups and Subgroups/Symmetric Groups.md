---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Symmetric Groups/"}
---


# Symmetric Groups

## Introduction

Permutation groups are not just another class of examples; they are central to the entire theory of finite groups. The symmetric groups provide concrete realizations of abstract group theory and are fundamental to understanding all finite groups.

## Definition

### Basic Definitions
- A **permutation** of a set $M$ is a bijection from $M$ to itself
- The set of all permutations of $M$ forms a group under function composition, called the **symmetric group** on $M$, denoted $\text{Sym}(M)$
- If $M = \{1, 2, \ldots, n\}$, the group is denoted $S_n$ and is called the **symmetric group on $n$ letters**
- Its order is $|S_n| = n!$
- A **permutation group** is any subgroup of a symmetric group

### Notation
Permutations are commonly written in **cycle notation**. A cycle $(a_1, a_2, \ldots, a_k)$ represents the permutation that sends $a_1 \to a_2$, $a_2 \to a_3$, ..., $a_k \to a_1$, and fixes all other elements.

Any permutation can be written as a product of disjoint cycles. For example, the permutation in $S_5$ that sends $1 \to 2$, $2 \to 5$, $5 \to 1$, $3 \to 4$, and $4 \to 3$ is written as $(1,2,5)(3,4)$.

## Examples

### Example 1: $S_3$ (Symmetric Group on 3 Letters)

The group $S_3$ has order $3! = 6$. Its elements are:

**Identity**: $e = ()$

**Transpositions** (2-cycles):
- $(1,2)$: swaps 1 and 2, fixes 3
- $(1,3)$: swaps 1 and 3, fixes 2
- $(2,3)$: swaps 2 and 3, fixes 1

**3-cycles**:
- $(1,2,3)$: sends $1 \to 2 \to 3 \to 1$
- $(1,3,2)$: sends $1 \to 3 \to 2 \to 1$

### Example 2: $S_4$ (Symmetric Group on 4 Letters)

The group $S_4$ has order $4! = 24$. Its elements include:

**Identity**: $e = ()$

**Transpositions**: $(1,2)$, $(1,3)$, $(1,4)$, $(2,3)$, $(2,4)$, $(3,4)$

**3-cycles**: $(1,2,3)$, $(1,2,4)$, $(1,3,2)$, $(1,3,4)$, $(1,4,2)$, $(1,4,3)$, $(2,3,4)$, $(2,4,3)$

**4-cycles**: $(1,2,3,4)$, $(1,2,4,3)$, $(1,3,2,4)$, $(1,3,4,2)$, $(1,4,2,3)$, $(1,4,3,2)$

**Products of disjoint transpositions**: $(1,2)(3,4)$, $(1,3)(2,4)$, $(1,4)(2,3)$

## Properties

### Order
The order of $S_n$ is $n!$.

### Non-abelian
Symmetric groups are non-abelian for $n \geq 3$. For example, in $S_3$:
- $(1,2)(1,3) = (1,3,2)$
- $(1,3)(1,2) = (1,2,3)$
- So $(1,2)(1,3) \neq (1,3)(1,2)$

### Center
The center of $S_n$ is trivial for $n \geq 3$.

### Conjugacy Classes
The conjugacy classes of $S_n$ correspond to cycle types. Two permutations are conjugate if and only if they have the same cycle type.

## Cayley's Theorem

**Theorem**: Every group is isomorphic to a subgroup of some symmetric group.

This theorem has profound implications. It establishes that every abstract group, no matter how it is defined (geometrically, through generators and relations, etc.), can be concretely realized as a group of permutations. This means that the study of permutation groups is, in a deep sense, the study of all groups.

### Proof Sketch
For a group $G$, consider the action of $G$ on itself by left multiplication. This gives a homomorphism from $G$ to $\text{Sym}(G)$, which is injective by the cancellation law.

## Cycle Structure

### Cycle Types
The cycle type of a permutation is the multiset of cycle lengths in its cycle decomposition. For example:
- $(1,2,3)(4,5)$ has cycle type $(3,2)$
- $(1,2)(3,4)(5,6)$ has cycle type $(2,2,2)$

### Sign of a Permutation
The **sign** of a permutation $\sigma$, denoted $\text{sgn}(\sigma)$, is:
- $+1$ if $\sigma$ can be written as a product of an even number of transpositions
- $-1$ if $\sigma$ can be written as a product of an odd number of transpositions

The sign function is a group homomorphism from $S_n$ to $\{1, -1\}$.

## Alternating Groups

### Definition
The **alternating group** $A_n$ is the kernel of the sign homomorphism:
$$A_n = \{\sigma \in S_n \mid \text{sgn}(\sigma) = 1\}$$

### Properties
- $A_n$ is a normal subgroup of $S_n$
- The order of $A_n$ is $\frac{n!}{2}$
- $A_n$ is simple for $n \geq 5$

## Applications

### Applications in Group Theory
- Understanding the structure of finite groups
- Providing concrete examples for abstract concepts
- Basis for Cayley's theorem

### Applications in Combinatorics
- Counting problems
- Enumeration of permutations with certain properties

### Applications in Physics
- Quantum mechanics (identical particles)
- Statistical mechanics

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Group Axioms\|Group Axioms]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Subgroups\|Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/4 - Jordan-Hölder Theorem/Alternating Groups\|Alternating Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Group Actions\|Group Actions]]
- [[Cayley's Theorem\|Cayley's Theorem]] 