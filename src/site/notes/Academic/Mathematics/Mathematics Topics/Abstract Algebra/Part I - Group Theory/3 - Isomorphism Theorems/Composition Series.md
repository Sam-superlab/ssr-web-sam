---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Composition Series/"}
---


# Composition Series

## Introduction

Composition series allow us to break down finite groups into simple building blocks, analogous to prime factorization of integers. This process is fundamental to understanding the structure of finite groups.

## Definition

**Definition 3.5**: A **subnormal series** of a group $G$ is a finite sequence of subgroups:

$$\{e\} = H_0 \trianglelefteq H_1 \trianglelefteq \cdots \trianglelefteq H_n = G$$

where each $H_i$ is a normal subgroup of $H_{i+1}$. The quotient groups $H_{i+1}/H_i$ are called the **factors** of the series.

A **composition series** is a subnormal series where all the factors $H_{i+1}/H_i$ are simple groups.

## Existence

The existence of a composition series for every finite group can be shown by starting with $G$ and finding a maximal normal subgroup $H_{n-1}$; then finding a maximal normal subgroup of $H_{n-1}$, and so on, until the trivial group is reached. The maximality at each step ensures the corresponding factor group is simple.

## Analogy with Prime Factorization

This process is analogous to the prime factorization of an integer. An integer is factored into primes; a finite group is "factored" via a composition series into simple groups. This analogy provides the entire motivation for one of the monumental achievements of 20th-century mathematics: the classification of all finite simple groups.

Just as understanding prime numbers is key to number theory, understanding simple groups is key to understanding all finite groups.

## Examples

### Example 1: Composition Series of $\mathbb{Z}_{12}$

A composition series for $\mathbb{Z}_{12}$ is:
$$\{0\} \trianglelefteq \langle 6 \rangle \trianglelefteq \langle 2 \rangle \trianglelefteq \mathbb{Z}_{12}$$

The factors are:
- $\langle 6 \rangle / \{0\} \cong \mathbb{Z}_2$
- $\langle 2 \rangle / \langle 6 \rangle \cong \mathbb{Z}_3$
- $\mathbb{Z}_{12} / \langle 2 \rangle \cong \mathbb{Z}_2$

### Example 2: Composition Series of $S_4$

A composition series for $S_4$ is:
$$\{e\} \trianglelefteq V \trianglelefteq A_4 \trianglelefteq S_4$$

where $V = \{e, (1,2)(3,4), (1,3)(2,4), (1,4)(2,3)\}$ is the Klein four-group.

The factors are:
- $V / \{e\} \cong \mathbb{Z}_2 \times \mathbb{Z}_2$
- $A_4 / V \cong \mathbb{Z}_3$
- $S_4 / A_4 \cong \mathbb{Z}_2$

### Example 3: Composition Series of $\mathbb{Z}_8$

A composition series for $\mathbb{Z}_8$ is:
$$\{0\} \trianglelefteq \langle 4 \rangle \trianglelefteq \langle 2 \rangle \trianglelefteq \mathbb{Z}_8$$

The factors are:
- $\langle 4 \rangle / \{0\} \cong \mathbb{Z}_2$
- $\langle 2 \rangle / \langle 4 \rangle \cong \mathbb{Z}_2$
- $\mathbb{Z}_8 / \langle 2 \rangle \cong \mathbb{Z}_2$

### Example 4: Composition Series of $D_4$

A composition series for $D_4$ is:
$$\{e\} \trianglelefteq \langle r^2 \rangle \trianglelefteq \langle r \rangle \trianglelefteq D_4$$

The factors are:
- $\langle r^2 \rangle / \{e\} \cong \mathbb{Z}_2$
- $\langle r \rangle / \langle r^2 \rangle \cong \mathbb{Z}_2$
- $D_4 / \langle r \rangle \cong \mathbb{Z}_2$

## Properties

### Length
The length of a composition series is the number of factors (simple groups) in the series.

### Factors
The composition factors are simple groups, which are the "building blocks" of the group.

### Uniqueness
While the composition series itself may not be unique, the composition factors are unique up to isomorphism and order (Jordan-Hölder Theorem).

## Jordan-Hölder Theorem

**Theorem 4.1 (Jordan-Hölder)**: Any two composition series of a given finite group have the same length. Furthermore, the sets of composition factors are isomorphic, up to a permutation of their order.

This profound result guarantees that the simple "building blocks" of any finite group are an intrinsic property of that group, independent of the specific way it is decomposed. The set of simple groups that appear in a composition series is a fundamental invariant, much like the set of prime factors of an integer.

## Applications

### Application 1: Understanding Group Structure

Composition series help us understand the structure of groups by breaking them down into simple components.

### Application 2: Classification of Groups

Composition series are fundamental to the classification of finite groups, which is one of the major achievements of 20th-century mathematics.

### Application 3: Solvability

A group is solvable if and only if all its composition factors are abelian (specifically, cyclic of prime order).

### Application 4: Galois Theory

Composition series are important in Galois theory, particularly in understanding the solvability of polynomial equations by radicals.

## Infinite Groups

While every finite group has a composition series, this is not true for infinite groups. For example, the additive group of integers $\mathbb{Z}$ has no composition series.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Simple Groups\|Simple Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/4 - Jordan-Hölder Theorem/Jordan-Hölder Theorem\|Jordan-Hölder Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/8 - Commutator Subgroups/Solvable Groups\|Solvable Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Quotient Groups\|Quotient Groups]] 