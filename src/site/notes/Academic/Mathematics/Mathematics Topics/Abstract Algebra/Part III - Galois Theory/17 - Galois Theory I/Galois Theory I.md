---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part III - Galois Theory/17 - Galois Theory I/Galois Theory I/"}
---


# Galois Theory I: The Fundamental Theorem

## Introduction

We now arrive at the heart of the course, which establishes the remarkable dictionary between field theory and group theory. Galois theory reveals a stunning and deep connection between the symmetries of the roots of a polynomial and the structure of the field extensions generated by those roots. This correspondence allows us to translate difficult problems about fields into more manageable problems about finite groups, ultimately answering the classical question of which polynomial equations can be solved by radicals.

## Galois Extensions and Galois Groups

### Definition of Galois Extension

A field extension $L/K$ is called a **Galois extension** if it is:
1. **Normal**: Every irreducible polynomial in $K[x]$ that has at least one root in $L$ splits completely in $L$
2. **Separable**: Every element in $L$ is separable over $K$ (its minimal polynomial has no repeated roots)

For finite extensions, these conditions are equivalent to saying that $L$ is the splitting field of a separable polynomial over $K$.

### Definition of Galois Group

**Definition 17.1**: Let $L/K$ be a Galois extension. The **Galois group** of the extension, denoted $\text{Gal}(L/K)$, is the group of all automorphisms of $L$ that fix every element of $K$. The group operation is function composition.

### Key Properties

For a finite Galois extension, the order of the Galois group is equal to the degree of the extension:

$$|\text{Gal}(L/K)| = [L : K]$$

## The Fundamental Theorem of Galois Theory

**Theorem 17.2 (The Fundamental Theorem of Galois Theory)**: Let $L/K$ be a finite Galois extension with Galois group $G = \text{Gal}(L/K)$. There is a one-to-one correspondence between the set of intermediate fields $E$ (where $K \subseteq E \subseteq L$) and the set of subgroups $H$ of $G$. The correspondence is given by:

- To each intermediate field $E$, we associate the subgroup of automorphisms that fix $E$: $H = \text{Gal}(L/E)$
- To each subgroup $H \leq G$, we associate its fixed field: $E = L^H = \{x \in L \mid \sigma(x) = x \text{ for all } \sigma \in H\}$

### Properties of the Correspondence

This correspondence has the following properties:

1. **Inclusion-Reversing**: If $E_1 \subseteq E_2$, then $\text{Gal}(L/E_2) \leq \text{Gal}(L/E_1)$. Conversely, if $H_1 \leq H_2$, then $L^{H_2} \subseteq L^{H_1}$.

2. **Degrees and Indices**: $[L : E] = |H|$ and $[E : K] = [G : H]$.

3. **Normality**: The extension $E/K$ is a normal (and thus Galois) extension if and only if its corresponding subgroup $H = \text{Gal}(L/E)$ is a normal subgroup of $G$. In this case, the Galois group of $E/K$ is isomorphic to the quotient group $G/H$:

$$\text{Gal}(E/K) \cong G/H$$

## Examples

### Example 1: Quadratic Extensions

Consider the extension $\mathbb{Q}(\sqrt{2})/\mathbb{Q}$. This is a Galois extension because:
- It is the splitting field of the separable polynomial $x^2 - 2$
- The Galois group $\text{Gal}(\mathbb{Q}(\sqrt{2})/\mathbb{Q})$ has order 2

The Galois group consists of two automorphisms:
- The identity map: $\sigma_1(a + b\sqrt{2}) = a + b\sqrt{2}$
- The conjugation map: $\sigma_2(a + b\sqrt{2}) = a - b\sqrt{2}$

The subgroups of $\text{Gal}(\mathbb{Q}(\sqrt{2})/\mathbb{Q})$ are:
- $\{e\}$ (trivial subgroup)
- $\text{Gal}(\mathbb{Q}(\sqrt{2})/\mathbb{Q})$ (the whole group)

The corresponding intermediate fields are:
- $L^{\{e\}} = \mathbb{Q}(\sqrt{2})$ (the whole field)
- $L^{\text{Gal}(\mathbb{Q}(\sqrt{2})/\mathbb{Q})} = \mathbb{Q}$ (the base field)

### Example 2: Cyclotomic Extensions

Consider the extension $\mathbb{Q}(\zeta_5)/\mathbb{Q}$, where $\zeta_5$ is a primitive 5th root of unity. This is a Galois extension because it is the splitting field of the cyclotomic polynomial $\Phi_5(x) = x^4 + x^3 + x^2 + x + 1$.

The Galois group $\text{Gal}(\mathbb{Q}(\zeta_5)/\mathbb{Q})$ is isomorphic to $\mathbb{Z}_4^* \cong \mathbb{Z}_4$, with elements:
- $\sigma_1: \zeta_5 \mapsto \zeta_5$
- $\sigma_2: \zeta_5 \mapsto \zeta_5^2$
- $\sigma_3: \zeta_5 \mapsto \zeta_5^3$
- $\sigma_4: \zeta_5 \mapsto \zeta_5^4$

The subgroups are:
- $\{e\}$
- $\{e, \sigma_2^2\}$ (order 2)
- $\text{Gal}(\mathbb{Q}(\zeta_5)/\mathbb{Q})$ (order 4)

### Example 3: The Splitting Field of $x^3 - 2$

Consider the polynomial $f(x) = x^3 - 2$ over $\mathbb{Q}$. Its splitting field is $L = \mathbb{Q}(\sqrt[3]{2}, \omega)$, where $\omega = e^{2\pi i/3}$ is a primitive cube root of unity.

The Galois group $\text{Gal}(L/\mathbb{Q})$ is isomorphic to $S_3$ (the symmetric group on 3 letters), with order 6.

The intermediate fields correspond to the subgroups of $S_3$:
- $\mathbb{Q}(\sqrt[3]{2})$ corresponds to a subgroup of order 2
- $\mathbb{Q}(\omega)$ corresponds to a subgroup of order 3
- $\mathbb{Q}$ corresponds to the whole group $S_3$

## Applications

### Application 1: Finding Intermediate Fields

The Fundamental Theorem provides a systematic way to find all intermediate fields of a Galois extension by finding all subgroups of the Galois group.

### Application 2: Determining Galois Groups

By understanding the structure of intermediate fields, we can often determine the structure of the Galois group.

### Application 3: Solvability by Radicals

The Fundamental Theorem is the key tool for determining whether a polynomial is solvable by radicals, as we will see in the next chapter.

## The Correspondence Theorem

The Fundamental Theorem also establishes a one-to-one correspondence between the subgroups of $G$ and the intermediate fields of the extension. This is sometimes called the **Correspondence Theorem** or **Lattice Theorem**.

### Lattice Structure

The correspondence preserves the lattice structure:
- If $H_1 \leq H_2 \leq G$, then $L^{H_2} \subseteq L^{H_1} \subseteq L$
- The intersection of subgroups corresponds to the compositum of fields
- The subgroup generated by a union corresponds to the intersection of fields

## Historical Context

The Fundamental Theorem of Galois Theory was discovered by Évariste Galois in the early 19th century, though it was not fully understood until later. It represents one of the most beautiful and powerful results in mathematics, connecting two seemingly unrelated areas: field theory and group theory.

The theorem was motivated by the problem of determining which polynomial equations can be solved by radicals. Galois realized that the solvability of a polynomial is determined by the structure of its Galois group, and the Fundamental Theorem provides the precise correspondence needed to make this connection.

## Summary

The Fundamental Theorem of Galois Theory establishes a perfect dictionary between field theory and group theory. It allows us to translate questions about fields (which can be infinite and complex) into questions about finite groups (which are more structured and often easier to analyze). This theorem is the foundation for understanding the solvability of polynomial equations and represents one of the crowning achievements of abstract algebra. 