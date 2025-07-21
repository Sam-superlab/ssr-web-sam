---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Third Isomorphism Theorem/"}
---


# Third Isomorphism Theorem

## Introduction

The Third Isomorphism Theorem provides a "cancellation" rule for quotients and establishes a one-to-one correspondence between the subgroups of a quotient group and the subgroups of the original group that contain the normal subgroup.

## Statement

**Theorem 3.3 (Third Isomorphism Theorem)**: Let $G$ be a group and let $N$ and $K$ be normal subgroups of $G$ with $N \subseteq K$. Then $N$ is a normal subgroup of $K$, $K/N$ is a normal subgroup of $G/N$, and the following isomorphism holds:

$$(G/N)/(K/N) \cong G/K$$

## Proof Sketch

The proof involves constructing a homomorphism and applying the First Isomorphism Theorem:

1. **Define the homomorphism**: Define $\phi: G/N \to G/K$ by $\phi(gN) = gK$.

2. **Show it's well-defined**: If $gN = g'N$, then $g^{-1}g' \in N \subseteq K$, so $gK = g'K$.

3. **Show it's a homomorphism**: $\phi((gN)(hN)) = \phi(ghN) = ghK = (gK)(hK) = \phi(gN)\phi(hN)$.

4. **Find kernel and image**: $\ker(\phi) = K/N$ and $\text{Im}(\phi) = G/K$.

5. **Apply First Isomorphism Theorem**: $(G/N)/\ker(\phi) \cong \text{Im}(\phi)$, so $(G/N)/(K/N) \cong G/K$.

## Examples

### Example 1: Integers

Let $G = \mathbb{Z}$, $N = 12\mathbb{Z}$, and $K = 4\mathbb{Z}$.

- $G/N = \mathbb{Z}/12\mathbb{Z}$
- $K/N = 4\mathbb{Z}/12\mathbb{Z} \cong \mathbb{Z}_3$
- $G/K = \mathbb{Z}/4\mathbb{Z}$
- By the Third Isomorphism Theorem: $(\mathbb{Z}/12\mathbb{Z})/(4\mathbb{Z}/12\mathbb{Z}) \cong \mathbb{Z}/4\mathbb{Z}$

### Example 2: Cyclic Groups

Let $G = \mathbb{Z}_{24}$, $N = \langle 8 \rangle = \{0, 8, 16\}$, and $K = \langle 4 \rangle = \{0, 4, 8, 12, 16, 20\}$.

- $G/N = \mathbb{Z}_{24}/\langle 8 \rangle \cong \mathbb{Z}_8$
- $K/N = \langle 4 \rangle/\langle 8 \rangle \cong \mathbb{Z}_2$
- $G/K = \mathbb{Z}_{24}/\langle 4 \rangle \cong \mathbb{Z}_4$
- By the Third Isomorphism Theorem: $\mathbb{Z}_8/\mathbb{Z}_2 \cong \mathbb{Z}_4$

### Example 3: Symmetric Groups

Let $G = S_4$, $N = V$ (Klein four-group), and $K = A_4$.

- $G/N = S_4/V$
- $K/N = A_4/V \cong \mathbb{Z}_3$
- $G/K = S_4/A_4 \cong \mathbb{Z}_2$
- By the Third Isomorphism Theorem: $(S_4/V)/(A_4/V) \cong S_4/A_4 \cong \mathbb{Z}_2$

## Correspondence Theorem

The Third Isomorphism Theorem also establishes the **Correspondence Theorem** (or **Lattice Theorem**), which provides a one-to-one correspondence between:

- Subgroups of $G/N$
- Subgroups of $G$ that contain $N$

### Statement of Correspondence Theorem

Let $G$ be a group and $N$ a normal subgroup of $G$. Then there is a one-to-one, inclusion-preserving correspondence between:

1. Subgroups of $G/N$
2. Subgroups of $G$ that contain $N$

Under this correspondence:
- Normal subgroups correspond to normal subgroups
- The index is preserved: $[G : H] = [G/N : H/N]$ for $H \supseteq N$

## Applications

### Application 1: Understanding Quotient Structure

The Third Isomorphism Theorem helps us understand the structure of quotient groups by relating them to simpler quotients.

### Application 2: Simplifying Quotients

The theorem provides a way to "cancel" normal subgroups in quotient expressions.

### Application 3: Subgroup Lattices

The Correspondence Theorem helps us understand the subgroup structure of quotient groups.

### Application 4: Galois Theory

The Correspondence Theorem is fundamental in Galois theory, where it corresponds to the relationship between intermediate fields and subgroups of the Galois group.

## Special Cases

### Case 1: $N = \{e\}$

If $N = \{e\}$, then $G/N = G$ and the theorem becomes the trivial statement $G/K \cong G/K$.

### Case 2: $K = G$

If $K = G$, then $G/K = \{e\}$ and the theorem becomes $(G/N)/(G/N) \cong \{e\}$.

### Case 3: $N = K$

If $N = K$, then $K/N = \{e\}$ and the theorem becomes $(G/N)/\{e\} \cong G/N$.

## Related Theorems

### First Isomorphism Theorem
Relates $G/\ker(\phi)$ to $\text{Im}(\phi)$ for homomorphisms $\phi: G \to H$.

### Second Isomorphism Theorem
Relates $(SN)/N$ to $S/(S \cap N)$ for subgroups $S$ and normal subgroups $N$.

## Summary

The Third Isomorphism Theorem provides a powerful tool for understanding quotient groups and their relationships. It is particularly useful for simplifying complex quotient expressions and understanding the structure of groups through their quotients. The associated Correspondence Theorem is fundamental for understanding subgroup lattices and has important applications in Galois theory.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/First Isomorphism Theorem\|First Isomorphism Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Second Isomorphism Theorem\|Second Isomorphism Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Quotient Groups\|Quotient Groups]]
- [[Correspondence Theorem\|Correspondence Theorem]] 