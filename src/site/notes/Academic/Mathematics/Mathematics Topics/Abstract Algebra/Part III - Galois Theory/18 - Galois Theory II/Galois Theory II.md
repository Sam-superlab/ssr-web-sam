---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part III - Galois Theory/18 - Galois Theory II/Galois Theory II/"}
---


# Galois Theory II: The Proof

## Introduction

The proof of the Fundamental Theorem of Galois Theory relies on a series of lemmas and propositions that connect the size of the automorphism group to the degree of the extension. This chapter provides a detailed outline of the proof.

## Proof Outline

### Step 1: Establish Equivalence for Galois Extensions

First, one proves the equivalence of the defining properties of a finite Galois extension:

1. It is normal and separable
2. It is the splitting field of a separable polynomial
3. $|\text{Aut}(L/K)| = [L:K]$
4. The fixed field of $\text{Aut}(L/K)$ is $K$

The key lemma, due to Artin, states that for any finite group of automorphisms $H$ of a field $L$, the extension $L/L^H$ is Galois with group $H$ and degree $|H|$.

### Step 2: Show the Correspondence is Bijective

With these equivalences, one shows that the maps $E \mapsto \text{Gal}(L/E)$ and $H \mapsto L^H$ are inverses of each other. The fact that $L^{\text{Gal}(L/E)} = E$ follows because $L/E$ is itself a Galois extension. The fact that $\text{Gal}(L/L^H) = H$ is a direct consequence of Artin's lemma.

### Step 3: Prove the Properties

The properties of the correspondence (inclusion-reversal, degrees/indices, and normality) are then proven using the established bijection and the definitions of degree, index, and normal subgroups.

## Key Lemmas

### Artin's Lemma

**Lemma 18.1 (Artin's Lemma)**: Let $L$ be a field and let $H$ be a finite group of automorphisms of $L$. Let $K = L^H$ be the fixed field of $H$. Then:

1. $L/K$ is a Galois extension
2. $\text{Gal}(L/K) = H$
3. $[L:K] = |H|$

### Proof of Artin's Lemma

The proof involves several steps:

1. **Show that $L/K$ is algebraic**: Every element of $L$ is algebraic over $K$
2. **Show that $L/K$ is separable**: The minimal polynomial of any element has distinct roots
3. **Show that $L/K$ is normal**: Every irreducible polynomial with a root in $L$ splits in $L$
4. **Show that $H = \text{Gal}(L/K)$**: Every element of $H$ is a $K$-automorphism, and every $K$-automorphism is in $H$

### Dedekind's Lemma

**Lemma 18.2 (Dedekind's Lemma)**: Let $L$ be a field and let $\sigma_1, \sigma_2, \ldots, \sigma_n$ be distinct automorphisms of $L$. Then $\sigma_1, \sigma_2, \ldots, \sigma_n$ are linearly independent over $L$.

This lemma is crucial for showing that the number of automorphisms cannot exceed the degree of the extension.

## The Correspondence

### Definition of the Maps

Let $L/K$ be a finite Galois extension with Galois group $G = \text{Gal}(L/K)$. We define two maps:

1. **Field to Group**: For each intermediate field $E$ (where $K \subseteq E \subseteq L$), we associate the subgroup of automorphisms that fix $E$: $H = \text{Gal}(L/E)$
2. **Group to Field**: For each subgroup $H \leq G$, we associate its fixed field: $E = L^H = \{x \in L \mid \sigma(x) = x \text{ for all } \sigma \in H\}$

### Bijectivity

**Theorem 18.3**: The maps $E \mapsto \text{Gal}(L/E)$ and $H \mapsto L^H$ are inverses of each other.

**Proof**: 
- For any intermediate field $E$, we have $L^{\text{Gal}(L/E)} = E$ because $L/E$ is a Galois extension
- For any subgroup $H \leq G$, we have $\text{Gal}(L/L^H) = H$ by Artin's lemma

## Properties of the Correspondence

### Inclusion-Reversing

**Theorem 18.4**: The correspondence is inclusion-reversing:
- If $E_1 \subseteq E_2$, then $\text{Gal}(L/E_2) \leq \text{Gal}(L/E_1)$
- Conversely, if $H_1 \leq H_2$, then $L^{H_2} \subseteq L^{H_1}$

### Degrees and Indices

**Theorem 18.5**: For any intermediate field $E$ and corresponding subgroup $H = \text{Gal}(L/E)$:
- $[L:E] = |H|$
- $[E:K] = [G:H]$

### Normality

**Theorem 18.6**: The extension $E/K$ is a normal (and thus Galois) extension if and only if its corresponding subgroup $H = \text{Gal}(L/E)$ is a normal subgroup of $G$. In this case, the Galois group of $E/K$ is isomorphic to the quotient group $G/H$:

$$\text{Gal}(E/K) \cong G/H$$

## Applications of the Proof

### Application 1: Understanding Field Structure

The proof shows how the structure of the Galois group reflects the structure of the field extension, providing a powerful tool for understanding field theory.

### Application 2: Computing Galois Groups

The correspondence allows us to compute Galois groups by understanding the intermediate fields and their relationships.

### Application 3: Solvability by Radicals

The proof provides the foundation for understanding when polynomial equations can be solved by radicals, as the structure of the Galois group determines the solvability.

## Examples

### Example 1: Quadratic Extensions

For the extension $\mathbb{Q}(\sqrt{2})/\mathbb{Q}$:
- The Galois group is $\{id, \sigma\}$ where $\sigma(\sqrt{2}) = -\sqrt{2}$
- The only intermediate field is $\mathbb{Q}$ itself
- The correspondence is: $\mathbb{Q} \leftrightarrow \{id, \sigma\}$

### Example 2: Cubic Extensions

For the extension $\mathbb{Q}(\sqrt[3]{2}, \omega)/\mathbb{Q}$:
- The Galois group is $S_3$ (the symmetric group on 3 letters)
- The intermediate fields correspond to the subgroups of $S_3$
- The normal subgroups correspond to normal extensions

### Example 3: Cyclotomic Extensions

For the extension $\mathbb{Q}(\zeta_n)/\mathbb{Q}$ where $\zeta_n$ is a primitive $n$-th root of unity:
- The Galois group is isomorphic to $(\mathbb{Z}/n\mathbb{Z})^\times$
- The intermediate fields correspond to the subgroups of this group
- All intermediate fields are normal over $\mathbb{Q}$

## Summary

The proof of the Fundamental Theorem of Galois Theory is a beautiful synthesis of field theory and group theory. It establishes a precise correspondence between the structure of field extensions and the structure of groups, providing a powerful tool for understanding both subjects.

The key insight is that the automorphisms of a field extension form a group that encodes the structure of the extension, and this group-theoretic information can be used to understand the field-theoretic properties.

This correspondence is fundamental to modern algebra and has applications throughout mathematics, from number theory to algebraic geometry to cryptography. 