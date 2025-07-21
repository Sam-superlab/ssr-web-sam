---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Cosets and Lagrange's Theorem/"}
---


# Cosets, Lagrange's Theorem, and Quotient Groups

## Introduction

After defining groups and subgroups, the next step is to understand their internal structure. This is achieved by analyzing how a subgroup partitions the larger group into equal-sized pieces, which leads to the first major theorem of finite group theory.

## Cosets

A subgroup $H$ of a group $G$ provides a natural way to partition the elements of $G$.

### Definition

**Definition 2.1**: Let $H$ be a subgroup of a group $G$, and let $g \in G$.

- The **left coset** of $H$ with respect to $g$ is the set $gH = \{gh \mid h \in H\}$
- The **right coset** of $H$ with respect to $g$ is the set $Hg = \{hg \mid h \in H\}$
- The element $g$ is called a **coset representative**

### Key Properties of Cosets

1. **Partition Property**: The left cosets of $H$ in $G$ form a partition of the set $G$. This means that:
   - Every element of $G$ belongs to exactly one left coset
   - Any two left cosets are either identical or disjoint

2. **Equivalence Relation**: This can be proven formally by showing that the relation $a \sim b$ if and only if $a^{-1}b \in H$ is an equivalence relation on $G$, where the equivalence classes are precisely the left cosets of $H$.

3. **Equal Cardinality**: There is a simple bijection between any subgroup $H$ and any of its cosets $gH$ (given by the map $h \mapsto gh$). This implies that all cosets of $H$ have the same cardinality as $H$ itself.

### Example: Cosets in $D_4$

Consider the dihedral group $D_4$ and the subgroup $H = \{e, r^2\}$ (rotations by $0°$ and $180°$):

- $eH = \{e \cdot e, e \cdot r^2\} = \{e, r^2\}$
- $rH = \{r \cdot e, r \cdot r^2\} = \{r, r^3\}$
- $sH = \{s \cdot e, s \cdot r^2\} = \{s, sr^2\}$
- $srH = \{sr \cdot e, sr \cdot r^2\} = \{sr, sr^3\}$

These four cosets partition $D_4$ into equal-sized pieces, each containing 2 elements.

## Lagrange's Theorem

This partitioning of a finite group into equal-sized pieces leads directly to a powerful and elegant result about the orders of subgroups.

### Statement

**Theorem 2.2 (Lagrange's Theorem)**: If $G$ is a finite group and $H$ is a subgroup of $G$, then the order of $H$ divides the order of $G$.

### Proof

Let $|G| = m$ and $|H| = n$. The distinct left cosets of $H$ in $G$ partition the set $G$. Let there be $p$ distinct left cosets. Since each coset has the same number of elements as $H$, namely $n$, the total number of elements in $G$ is the sum of the elements in all the distinct cosets. Therefore, $m = np$. This shows that $n$ divides $m$.

### Index of a Subgroup

The number of distinct cosets, $p$, is called the **index** of $H$ in $G$, denoted $[G : H]$. The theorem can thus be stated as:

$$|G| = [G : H] \cdot |H|$$

### Consequences

Lagrange's Theorem is a cornerstone of finite group theory because it places a strong restriction on the possible sizes of subgroups. For instance, a group of order 30 can only have subgroups of orders 1, 2, 3, 5, 6, 10, 15, and 30.

### Important Note: Converse is False

The theorem is a one-way implication. The converse is not true in general: if $d$ is a divisor of $|G|$, there is not necessarily a subgroup of order $d$.

**Counterexample**: The alternating group $A_4$ has order 12 but contains no subgroup of order 6. This failure of the converse of Lagrange's Theorem is a deep and important feature of group structure, and it serves as a primary motivation for the Sylow Theorems (Chapter 7), which provide a partial converse for orders that are powers of a prime.

## Normal Subgroups and Quotient Groups

The set of cosets of a subgroup raises a natural question: can this set itself be endowed with a group structure?

### The Problem

Consider the set of left cosets, denoted $G/H$. A natural candidate for a binary operation is $(aH)(bH) = (ab)H$. For this operation to be well-defined, the result must be independent of the choice of representatives $a$ and $b$.

### Condition for Well-Defined Operation

This condition holds if and only if the subgroup's left and right cosets coincide for every element, i.e., $gH = Hg$ for all $g \in G$. This leads to a special class of subgroups.

### Definition of Normal Subgroup

**Definition 2.3**: A subgroup $N$ of a group $G$ is a **normal subgroup** if for every $g \in G$, $gNg^{-1} = N$. This is denoted by $N \trianglelefteq G$.

The condition $gNg^{-1} = N$ is equivalent to $gN = Ng$ for all $g \in G$.

### Quotient Groups

When a subgroup $N$ is normal, the set of its cosets, $G/N$, forms a group under the operation $(aN)(bN) = abN$. This group is called the **quotient group** or **factor group** of $G$ by $N$.

- The identity element is the coset $eN = N$
- The inverse of $aN$ is $a^{-1}N$

### Construction and Interpretation

The construction of a quotient group is a fundamental method for simplifying a group. It effectively "collapses" or "factors out" the structure of the normal subgroup $N$, treating all elements of $N$ as equivalent to the identity.

### Key Example: Integers Modulo n

A key example is the group of integers modulo $n$, $(\mathbb{Z}/n\mathbb{Z}, +)$, which is the quotient group of the integers $(\mathbb{Z}, +)$ by the normal subgroup $n\mathbb{Z}$.

- Elements: $\{0 + n\mathbb{Z}, 1 + n\mathbb{Z}, \ldots, (n-1) + n\mathbb{Z}\}$
- Operation: $(a + n\mathbb{Z}) + (b + n\mathbb{Z}) = (a + b) + n\mathbb{Z}$
- This construction is the foundation of modular arithmetic

## Examples

### Example 1: Normal Subgroups in Abelian Groups

In an abelian group, every subgroup is normal because $gng^{-1} = n$ for all $g, n \in G$.

### Example 2: Normal Subgroups in $D_4$

Consider the subgroup $N = \{e, r^2\}$ in $D_4$:
- For any rotation $r^k$: $r^k N = N r^k$ (since $r^2$ commutes with rotations)
- For any reflection $sr^k$: $(sr^k)N = N(sr^k)$ (since $r^2$ is in the center)

Therefore, $N$ is normal, and $D_4/N$ is a group of order 4.

### Example 3: The Alternating Group

The alternating group $A_n$ is a normal subgroup of the symmetric group $S_n$ because:
- $A_n$ is the kernel of the sign homomorphism $\text{sgn}: S_n \to \{\pm 1\}$
- The quotient group $S_n/A_n$ is isomorphic to $\{\pm 1\}$

## Applications

### Application 1: Order of Elements

Lagrange's Theorem can be used to find the order of elements. If $g \in G$ has order $k$, then $\langle g \rangle$ is a subgroup of order $k$, so $k$ must divide $|G|$.

### Application 2: Prime Order Groups

If $G$ is a group of prime order $p$, then by Lagrange's Theorem, the only possible subgroups are $\{e\}$ and $G$ itself. This implies that $G$ is cyclic and generated by any non-identity element.

### Application 3: Index Calculations

The index $[G : H]$ can be calculated as $[G : H] = |G|/|H|$, which is often useful in counting arguments.

## Summary

Cosets provide a natural way to partition a group using a subgroup, leading to Lagrange's Theorem which restricts the possible sizes of subgroups. Normal subgroups allow us to construct quotient groups, which are essential for understanding group structure and for applications in Galois theory. The concepts introduced here form the foundation for the isomorphism theorems and the deeper study of group structure. 