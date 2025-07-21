---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/4 - Jordan-Hölder Theorem/Alternating Groups/"}
---


# Alternating Groups

## Introduction

The alternating groups are a critical family of simple groups. They are fundamental to understanding the structure of symmetric groups and have profound implications for Galois theory.

## Definition

**Definition 4.2**: 
- A **permutation** is **even** if it can be written as a product of an even number of transpositions (2-cycles). It is **odd** otherwise.
- The **sign** of a permutation $\sigma$, denoted $\text{sgn}(\sigma)$, is $+1$ if $\sigma$ is even and $-1$ if $\sigma$ is odd.
- The map $\text{sgn}: S_n \to \{1, -1\}$ is a group homomorphism.
- The **alternating group** $A_n$ is the kernel of this homomorphism.

## Properties

As the kernel of a homomorphism, $A_n$ is a normal subgroup of $S_n$. Its index is $[S_n : A_n] = 2$, so its order is $|A_n| = n!/2$.

## Structural Properties

The structural properties of alternating groups are fundamental to the entire theory:

### Abelian Property
$A_n$ is abelian if and only if $n \leq 3$.

### Simplicity of $A_4$
$A_4$ is not simple. It contains a normal subgroup of order 4, the Klein four-group:
$$V = \{e, (1,2)(3,4), (1,3)(2,4), (1,4)(2,3)\}$$

### Simplicity for $n \geq 5$
**Theorem 4.3**: The alternating group $A_n$ is simple for all $n \geq 5$.

## Examples

### Example 1: $A_3$
The alternating group $A_3$ has order $3!/2 = 3$ and consists of:
- $e$ (identity)
- $(1,2,3)$ (3-cycle)
- $(1,3,2)$ (3-cycle)

$A_3$ is abelian and isomorphic to $\mathbb{Z}_3$.

### Example 2: $A_4$
The alternating group $A_4$ has order $4!/2 = 12$ and consists of:
- The identity
- All 3-cycles: $(1,2,3)$, $(1,2,4)$, $(1,3,2)$, $(1,3,4)$, $(1,4,2)$, $(1,4,3)$, $(2,3,4)$, $(2,4,3)$
- Products of two disjoint transpositions: $(1,2)(3,4)$, $(1,3)(2,4)$, $(1,4)(2,3)$

$A_4$ is not simple because it contains the Klein four-group as a normal subgroup.

### Example 3: $A_5$
The alternating group $A_5$ has order $5!/2 = 60$ and is simple. It contains:
- The identity
- All 3-cycles (20 elements)
- All 5-cycles (24 elements)
- Products of two disjoint transpositions (15 elements)

## Historical Significance

The simplicity of $A_n$ for $n \geq 5$ is one of the most important results in elementary group theory. It is the deep structural reason behind the central result of Galois theory: the insolvability of the general polynomial equation of degree five or higher.

A group is called "solvable" if its composition factors are all abelian (specifically, cyclic of prime order). Since $A_5$ is a non-abelian simple group, any group having $A_5$ as a composition factor cannot be solvable.

The Galois group of a general quintic polynomial is $S_5$, which has the composition series:
$$\{e\} \trianglelefteq A_5 \trianglelefteq S_5$$

The factors are:
- $A_5/\{e\} \cong A_5$ (not abelian)
- $S_5/A_5 \cong \mathbb{Z}_2$ (abelian)

Because the factor $A_5$ is not abelian, the group $S_5$ is not solvable, which ultimately proves the impossibility of a general quintic formula involving only radicals.

## Applications

### Application 1: Galois Theory
The simplicity of $A_n$ for $n \geq 5$ is crucial for understanding the insolvability of polynomial equations of degree 5 or higher.

### Application 2: Group Classification
Alternating groups are fundamental examples of simple groups and are essential to the classification of finite simple groups.

### Application 3: Symmetry
Alternating groups represent the "even" symmetries of objects, which are often more fundamental than the full symmetric group.

### Application 4: Combinatorics
Alternating groups are important in combinatorics, particularly in the study of permutations and their properties.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Symmetric Groups\|Symmetric Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Simple Groups\|Simple Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Group Homomorphisms\|Group Homomorphisms]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/8 - Commutator Subgroups/Solvable Groups\|Solvable Groups]] 