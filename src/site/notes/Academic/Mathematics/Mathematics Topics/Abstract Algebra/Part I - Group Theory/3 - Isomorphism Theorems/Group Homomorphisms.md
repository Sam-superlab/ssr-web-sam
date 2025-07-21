---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Group Homomorphisms/"}
---


# Group Homomorphisms

## Introduction

A **homomorphism** is a map between groups that preserves the group structure. Homomorphisms are fundamental to understanding the relationships between groups and are essential for the isomorphism theorems.

## Definition

A **homomorphism** is a map $\phi: G \to H$ between two groups that preserves the group structure, meaning $\phi(g_1 g_2) = \phi(g_1) \phi(g_2)$ for all $g_1, g_2 \in G$.

## Important Sets Associated with Homomorphisms

Two important sets associated with a homomorphism are:

### 1. Kernel
The **kernel** of $\phi$ is the set of elements in $G$ that map to the identity in $H$:
$$\ker(\phi) = \{g \in G \mid \phi(g) = e_H\}$$

**Properties**:
- The kernel is always a normal subgroup of $G$
- $\phi$ is injective if and only if $\ker(\phi) = \{e_G\}$

### 2. Image
The **image** of $\phi$ is the set of elements in $H$ that are mapped to by some element in $G$:
$$\text{Im}(\phi) = \{\phi(g) \mid g \in G\}$$

**Properties**:
- The image is always a subgroup of $H$
- $\phi$ is surjective if and only if $\text{Im}(\phi) = H$

## Examples

### Example 1: Homomorphism from $\mathbb{Z}$ to $\mathbb{Z}_6$

Consider the homomorphism $\phi: \mathbb{Z} \to \mathbb{Z}_6$ defined by $\phi(n) = n \bmod 6$.

- **Kernel**: $\ker(\phi) = 6\mathbb{Z} = \{0, \pm6, \pm12, \ldots\}$
- **Image**: $\text{Im}(\phi) = \mathbb{Z}_6$
- **Properties**: Surjective but not injective

### Example 2: Homomorphism from $\mathbb{R}^*$ to $\mathbb{R}^*$

Consider the homomorphism $\phi: \mathbb{R}^* \to \mathbb{R}^*$ defined by $\phi(x) = x^2$.

- **Kernel**: $\ker(\phi) = \{\pm 1\}$
- **Image**: $\text{Im}(\phi) = \mathbb{R}^+$ (positive real numbers)
- **Properties**: Neither injective nor surjective

### Example 3: Homomorphism from $S_n$ to $\{\pm 1\}$

Consider the sign homomorphism $\text{sgn}: S_n \to \{\pm 1\}$.

- **Kernel**: $\ker(\text{sgn}) = A_n$ (alternating group)
- **Image**: $\text{Im}(\text{sgn}) = \{\pm 1\}$
- **Properties**: Surjective but not injective for $n \geq 3$

### Example 4: Homomorphism from $GL_n(\mathbb{R})$ to $\mathbb{R}^*$

Consider the determinant homomorphism $\det: GL_n(\mathbb{R}) \to \mathbb{R}^*$.

- **Kernel**: $\ker(\det) = SL_n(\mathbb{R})$ (special linear group)
- **Image**: $\text{Im}(\det) = \mathbb{R}^*$
- **Properties**: Surjective but not injective

## Properties

### Basic Properties
1. **Identity preservation**: $\phi(e_G) = e_H$
2. **Inverse preservation**: $\phi(g^{-1}) = \phi(g)^{-1}$
3. **Power preservation**: $\phi(g^n) = \phi(g)^n$ for all $n \in \mathbb{Z}$

### Composition
If $\phi: G \to H$ and $\psi: H \to K$ are homomorphisms, then $\psi \circ \phi: G \to K$ is also a homomorphism.

### Restriction
If $\phi: G \to H$ is a homomorphism and $S$ is a subgroup of $G$, then the restriction $\phi|_S: S \to H$ is a homomorphism.

## Types of Homomorphisms

### Monomorphism
A homomorphism that is injective (one-to-one).

### Epimorphism
A homomorphism that is surjective (onto).

### Isomorphism
A homomorphism that is bijective (both injective and surjective).

### Endomorphism
A homomorphism from a group to itself.

### Automorphism
An isomorphism from a group to itself.

## Applications

### Application 1: Understanding Group Structure
Homomorphisms help us understand the structure of groups by relating them to other groups.

### Application 2: First Isomorphism Theorem
Homomorphisms are essential for the first isomorphism theorem, which states that $G/\ker(\phi) \cong \text{Im}(\phi)$.

### Application 3: Group Actions
Homomorphisms are fundamental to the study of group actions, where a group acts on a set.

### Application 4: Representation Theory
Homomorphisms into matrix groups are the basis of representation theory.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Isomorphism Theorems\|Isomorphism Theorems]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Quotient Groups\|Quotient Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Group Actions\|Group Actions]]
- [[Automorphisms\|Automorphisms]] 