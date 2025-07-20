---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Quotient Groups/"}
---


# Quotient Groups

## Introduction

When a subgroup $N$ is normal, the set of its cosets, $G/N$, forms a group under a natural operation. This construction is fundamental to group theory and provides a powerful method for understanding group structure.

## Definition

When a subgroup $N$ is normal, the set of its cosets, $G/N$, forms a group under the operation $(aN)(bN) = abN$. This group is called the **quotient group** or **factor group** of $G$ by $N$.

### Group Structure
- **Identity element**: The coset $eN = N$
- **Inverse**: The inverse of $aN$ is $a^{-1}N$
- **Operation**: $(aN)(bN) = abN$

## Construction and Interpretation

The construction of a quotient group is a fundamental method for simplifying a group. It effectively "collapses" or "factors out" the structure of the normal subgroup $N$, treating all elements of $N$ as equivalent to the identity.

### Well-Defined Operation
The operation $(aN)(bN) = abN$ is well-defined because $N$ is normal. This means that if $aN = a'N$ and $bN = b'N$, then $abN = a'b'N$.

## Key Example: Integers Modulo n

A key example is the group of integers modulo $n$, $(\mathbb{Z}/n\mathbb{Z}, +)$, which is the quotient group of the integers $(\mathbb{Z}, +)$ by the normal subgroup $n\mathbb{Z}$.

### Structure
- **Elements**: $\{0 + n\mathbb{Z}, 1 + n\mathbb{Z}, \ldots, (n-1) + n\mathbb{Z}\}$
- **Operation**: $(a + n\mathbb{Z}) + (b + n\mathbb{Z}) = (a + b) + n\mathbb{Z}$
- **Order**: $n$
- **Isomorphism**: $\mathbb{Z}/n\mathbb{Z} \cong \mathbb{Z}_n$

This construction is the foundation of modular arithmetic.

## Examples

### Example 1: Quotient Groups in Abelian Groups

In an abelian group, every subgroup is normal, so we can always form quotient groups.

**Example**: Consider $(\mathbb{Z}, +)$ and the subgroup $6\mathbb{Z}$:
- $\mathbb{Z}/6\mathbb{Z} = \{0 + 6\mathbb{Z}, 1 + 6\mathbb{Z}, 2 + 6\mathbb{Z}, 3 + 6\mathbb{Z}, 4 + 6\mathbb{Z}, 5 + 6\mathbb{Z}\}$
- This is isomorphic to $\mathbb{Z}_6$

### Example 2: Quotient Groups in $D_4$

Consider the normal subgroup $N = \{e, r^2\}$ in $D_4$:
- $D_4/N = \{N, rN, sN, srN\}$
- The operation is well-defined because $N$ is normal
- $D_4/N$ is a group of order 4

### Example 3: Quotient Groups in $S_n$

The alternating group $A_n$ is a normal subgroup of $S_n$:
- $S_n/A_n = \{A_n, (1,2)A_n\}$
- This is isomorphic to $\{\pm 1\}$ under multiplication

### Example 4: Quotient Groups in Matrix Groups

Consider the group $GL_n(\mathbb{R})$ and the normal subgroup $SL_n(\mathbb{R})$ (matrices with determinant 1):
- $GL_n(\mathbb{R})/SL_n(\mathbb{R}) \cong \mathbb{R}^*$ (the multiplicative group of non-zero real numbers)
- The isomorphism is given by $A \cdot SL_n(\mathbb{R}) \mapsto \det(A)$

## Properties

### Order
If $G$ is finite, then $|G/N| = |G|/|N| = [G : N]$.

### Abelian Quotients
If $G$ is abelian, then $G/N$ is abelian for any normal subgroup $N$.

### Cyclic Quotients
If $G$ is cyclic, then $G/N$ is cyclic for any normal subgroup $N$.

### Simple Groups
A group $G$ is simple if and only if its only normal subgroups are $\{e\}$ and $G$ itself.

## Applications

### Application 1: Group Structure
Quotient groups help us understand the structure of groups by "factoring out" normal subgroups.

### Application 2: Homomorphisms
Quotient groups are essential for the first isomorphism theorem, which states that $G/\ker(\phi) \cong \text{im}(\phi)$ for any homomorphism $\phi: G \to H$.

### Application 3: Galois Theory
Quotient groups are fundamental in Galois theory, where they correspond to intermediate fields.

### Application 4: Representation Theory
Quotient groups are important in representation theory and the study of group actions.

## The Natural Homomorphism

For any normal subgroup $N$ of $G$, there is a natural homomorphism $\pi: G \to G/N$ defined by $\pi(g) = gN$. This homomorphism is surjective and has kernel $N$.

### Properties
- $\pi$ is surjective
- $\ker(\pi) = N$
- $\text{im}(\pi) = G/N$

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Cosets\|Cosets]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Group Homomorphisms\|Group Homomorphisms]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Isomorphism Theorems\|Isomorphism Theorems]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Simple Groups\|Simple Groups]] 