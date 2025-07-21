---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Simple Groups/"}
---


# Simple Groups

## Introduction

Simple groups are the "atoms" of group theory. They cannot be simplified further by forming non-trivial quotient groups and are fundamental to understanding the structure of all finite groups.

## Definition

**Definition 3.4**: A group $G$ is **simple** if its only normal subgroups are the trivial subgroup $\{e\}$ and the group $G$ itself.

## Key Examples

### Cyclic Groups of Prime Order
The cyclic groups $\mathbb{Z}_p$ for a prime $p$ are simple.

**Proof**: If $H$ is a non-trivial subgroup of $\mathbb{Z}_p$, then $|H|$ divides $p$. Since $p$ is prime, $|H| = p$, so $H = \mathbb{Z}_p$.

### Alternating Groups
The alternating groups $A_n$ are simple for $n \geq 5$.

**Note**: $A_4$ is not simple because it contains the Klein four-group as a normal subgroup.

### Other Simple Groups
- **PSL groups**: Projective special linear groups over finite fields
- **Sporadic groups**: 26 exceptional simple groups
- **Lie type groups**: Groups related to Lie algebras

## Properties

### No Non-Trivial Quotients
A group $G$ is simple if and only if it has no non-trivial quotient groups (other than $G$ itself).

### No Non-Trivial Homomorphic Images
A group $G$ is simple if and only if every homomorphism from $G$ is either injective or trivial.

### Composition Series
Simple groups are the building blocks in composition series. Every finite group can be "factored" into simple groups.

## Classification of Finite Simple Groups

The classification of finite simple groups is one of the monumental achievements of 20th-century mathematics. It states that every finite simple group belongs to one of the following families:

### 1. Cyclic Groups of Prime Order
$\mathbb{Z}_p$ where $p$ is prime.

### 2. Alternating Groups
$A_n$ for $n \geq 5$.

### 3. Groups of Lie Type
Groups related to Lie algebras over finite fields, including:
- **PSL groups**: Projective special linear groups
- **PSU groups**: Projective special unitary groups
- **PSp groups**: Projective symplectic groups
- **Orthogonal groups**: Various orthogonal groups

### 4. Sporadic Groups
26 exceptional simple groups that don't fit into the other families, including:
- **Mathieu groups**: $M_{11}, M_{12}, M_{22}, M_{23}, M_{24}$
- **Monster group**: The largest sporadic simple group
- **Baby Monster**: Second largest sporadic simple group

## Applications

### Application 1: Group Structure
Simple groups are essential for understanding the structure of all finite groups through composition series.

### Application 2: Galois Theory
Simple groups are important in Galois theory, particularly in understanding the solvability of polynomial equations.

### Application 3: Representation Theory
Simple groups are fundamental to representation theory and the study of group actions.

### Application 4: Cryptography
Some cryptographic protocols are based on the difficulty of certain problems in simple groups.

## Examples

### Example 1: $\mathbb{Z}_5$ is Simple
The group $\mathbb{Z}_5$ has order 5, which is prime. Its only subgroups are $\{0\}$ and $\mathbb{Z}_5$ itself, so it is simple.

### Example 2: $A_5$ is Simple
The alternating group $A_5$ has order 60 and is simple. This is a key fact in the proof that the general quintic equation is not solvable by radicals.

### Example 3: $S_4$ is Not Simple
The symmetric group $S_4$ is not simple because it contains the alternating group $A_4$ as a normal subgroup.

### Example 4: $D_4$ is Not Simple
The dihedral group $D_4$ is not simple because it contains the subgroup $\{e, r^2\}$ as a normal subgroup.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Quotient Groups\|Quotient Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Composition Series\|Composition Series]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/4 - Jordan-Hölder Theorem/Jordan-Hölder Theorem\|Jordan-Hölder Theorem]]
- [[Classification of Finite Simple Groups\|Classification of Finite Simple Groups]] 