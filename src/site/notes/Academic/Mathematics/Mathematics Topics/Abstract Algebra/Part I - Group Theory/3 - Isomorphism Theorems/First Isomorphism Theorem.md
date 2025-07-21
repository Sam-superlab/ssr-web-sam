---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/First Isomorphism Theorem/"}
---


# First Isomorphism Theorem

## Introduction

The First Isomorphism Theorem is arguably the most important theorem in group theory. It provides a direct link between homomorphisms and quotient groups, showing that factoring a group by the kernel of a map precisely captures the structure of the map's image.

## Statement

**Theorem 3.1 (First Isomorphism Theorem)**: Let $\phi: G \to H$ be a group homomorphism. Then the quotient group $G/\ker(\phi)$ is isomorphic to the image of $\phi$.

$$G/\ker(\phi) \cong \text{Im}(\phi)$$

## Proof Sketch

The proof involves constructing an explicit isomorphism $\psi: G/\ker(\phi) \to \text{Im}(\phi)$ defined by $\psi(g\ker(\phi)) = \phi(g)$.

### Steps:
1. **Well-defined**: Show that if $g\ker(\phi) = g'\ker(\phi)$, then $\phi(g) = \phi(g')$
2. **Homomorphism**: Show that $\psi$ preserves the group operation
3. **Injective**: Show that $\ker(\psi) = \{\ker(\phi)\}$
4. **Surjective**: Show that every element in $\text{Im}(\phi)$ is in the image of $\psi$

## Examples

### Example 1: Integers Modulo n

Consider the homomorphism $\phi: \mathbb{Z} \to \mathbb{Z}_6$ defined by $\phi(n) = n \bmod 6$.

- $\ker(\phi) = 6\mathbb{Z}$
- $\text{Im}(\phi) = \mathbb{Z}_6$
- By the First Isomorphism Theorem: $\mathbb{Z}/6\mathbb{Z} \cong \mathbb{Z}_6$

### Example 2: Real Numbers

Consider the homomorphism $\phi: \mathbb{R}^* \to \mathbb{R}^*$ defined by $\phi(x) = x^2$.

- $\ker(\phi) = \{\pm 1\}$
- $\text{Im}(\phi) = \mathbb{R}^+$ (positive real numbers)
- By the First Isomorphism Theorem: $\mathbb{R}^* / \{\pm 1\} \cong \mathbb{R}^+$

### Example 3: Symmetric Groups

Consider the sign homomorphism $\text{sgn}: S_n \to \{\pm 1\}$.

- $\ker(\text{sgn}) = A_n$ (alternating group)
- $\text{Im}(\text{sgn}) = \{\pm 1\}$
- By the First Isomorphism Theorem: $S_n/A_n \cong \{\pm 1\}$

### Example 4: Matrix Groups

Consider the determinant homomorphism $\det: GL_n(\mathbb{R}) \to \mathbb{R}^*$.

- $\ker(\det) = SL_n(\mathbb{R})$ (special linear group)
- $\text{Im}(\det) = \mathbb{R}^*$
- By the First Isomorphism Theorem: $GL_n(\mathbb{R})/SL_n(\mathbb{R}) \cong \mathbb{R}^*$

## Applications

### Application 1: Understanding Group Structure

The First Isomorphism Theorem helps us understand the structure of groups by relating them to simpler groups through homomorphisms.

**Example**: If we have a homomorphism $\phi: G \to H$ with kernel $K$, then $G$ is "built" from $K$ and $H$ in a precise way.

### Application 2: Proving Isomorphisms

The theorem provides a powerful tool for proving that two groups are isomorphic without having to construct an explicit isomorphism.

**Example**: To show that $\mathbb{Z}/n\mathbb{Z} \cong \mathbb{Z}_n$, we can use the homomorphism $\phi: \mathbb{Z} \to \mathbb{Z}_n$ defined by $\phi(k) = k \bmod n$.

### Application 3: Classification of Groups

The theorem is essential for understanding the structure of groups and their classification.

**Example**: Understanding the structure of finite abelian groups through their decomposition into cyclic groups.

### Application 4: Galois Theory

The First Isomorphism Theorem is fundamental in Galois theory, where it helps understand the relationship between field extensions and their Galois groups.

## Special Cases

### Case 1: Injective Homomorphism
If $\phi: G \to H$ is injective, then $\ker(\phi) = \{e\}$, so $G/\{e\} \cong G \cong \text{Im}(\phi)$. This shows that $G$ is isomorphic to a subgroup of $H$.

### Case 2: Surjective Homomorphism
If $\phi: G \to H$ is surjective, then $\text{Im}(\phi) = H$, so $G/\ker(\phi) \cong H$. This shows that $H$ is isomorphic to a quotient of $G$.

### Case 3: Isomorphism
If $\phi: G \to H$ is an isomorphism, then $\ker(\phi) = \{e\}$ and $\text{Im}(\phi) = H$, so $G/\{e\} \cong G \cong H$.

## Related Theorems

### Second Isomorphism Theorem
Relates the quotient $(SN)/N$ to $S/(S \cap N)$ for subgroups $S$ and normal subgroups $N$.

### Third Isomorphism Theorem
Provides a "cancellation" rule for quotients: $(G/N)/(K/N) \cong G/K$.

## Summary

The First Isomorphism Theorem is a fundamental result that connects homomorphisms, normal subgroups, and quotient groups. It provides a powerful tool for understanding group structure and proving isomorphisms. The theorem is essential for the deeper study of group theory and its applications throughout mathematics.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Group Homomorphisms\|Group Homomorphisms]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Quotient Groups\|Quotient Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Second Isomorphism Theorem\|Second Isomorphism Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Third Isomorphism Theorem\|Third Isomorphism Theorem]] 