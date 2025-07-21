---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Second Isomorphism Theorem/"}
---


# Second Isomorphism Theorem

## Introduction

The Second Isomorphism Theorem, also known as the "Diamond Isomorphism Theorem" due to the shape of the corresponding subgroup lattice diagram, relates the quotient of a product of subgroups to the quotient of their intersection.

## Statement

**Theorem 3.2 (Second Isomorphism Theorem)**: Let $G$ be a group, $S$ a subgroup of $G$, and $N$ a normal subgroup of $G$. Then the product $SN = \{sn \mid s \in S, n \in N\}$ is a subgroup of $G$, the intersection $S \cap N$ is a normal subgroup of $S$, and the following isomorphism holds:

$$(SN)/N \cong S/(S \cap N)$$

## Proof Sketch

The proof involves several steps:

1. **Show $SN$ is a subgroup**: Use the subgroup test to verify that $SN$ is closed under the group operation and inverses.

2. **Show $S \cap N$ is normal in $S$**: For any $s \in S$ and $x \in S \cap N$, show that $sxs^{-1} \in S \cap N$.

3. **Construct the isomorphism**: Define a homomorphism $\phi: S \to (SN)/N$ by $\phi(s) = sN$ and show that its kernel is $S \cap N$.

4. **Apply the First Isomorphism Theorem**: Since $\ker(\phi) = S \cap N$ and $\text{Im}(\phi) = (SN)/N$, we get $S/(S \cap N) \cong (SN)/N$.

## Examples

### Example 1: Symmetric Groups

Let $G = S_4$, $S = \langle (1,2,3) \rangle$ (cyclic subgroup of order 3), and $N = A_4$ (alternating group).

- $SN = S_4$ (since $S_4 = A_4 \cup A_4(1,2,3)$)
- $S \cap N = \{e\}$
- By the Second Isomorphism Theorem: $S_4/A_4 \cong \langle (1,2,3) \rangle / \{e\} \cong \mathbb{Z}_3$

### Example 2: Dihedral Groups

Let $G = D_6$, $S = \langle r^2 \rangle$ (subgroup of rotations by multiples of $120°$), and $N = \langle r^3 \rangle$ (subgroup of rotations by multiples of $180°$).

- $SN = \langle r \rangle$ (all rotations)
- $S \cap N = \{e\}$
- By the Second Isomorphism Theorem: $\langle r \rangle / \langle r^3 \rangle \cong \langle r^2 \rangle / \{e\} \cong \mathbb{Z}_3$

### Example 3: Abelian Groups

Let $G = \mathbb{Z}_{12}$, $S = \langle 2 \rangle = \{0, 2, 4, 6, 8, 10\}$, and $N = \langle 3 \rangle = \{0, 3, 6, 9\}$.

- $SN = \mathbb{Z}_{12}$ (since $\gcd(2, 3) = 1$)
- $S \cap N = \langle 6 \rangle = \{0, 6\}$
- By the Second Isomorphism Theorem: $\mathbb{Z}_{12} / \langle 3 \rangle \cong \langle 2 \rangle / \langle 6 \rangle \cong \mathbb{Z}_3$

## Applications

### Application 1: Understanding Subgroup Structure

The Second Isomorphism Theorem helps us understand how subgroups interact with normal subgroups and their quotients.

### Application 2: Index Calculations

The theorem can be used to calculate indices: $[SN : N] = [S : S \cap N]$.

### Application 3: Proving Isomorphisms

The theorem provides a powerful tool for proving that two quotient groups are isomorphic.

## Special Cases

### Case 1: $S \cap N = \{e\}$

If $S \cap N = \{e\}$, then $(SN)/N \cong S$. This means that $S$ is isomorphic to a subgroup of $G/N$.

### Case 2: $S$ is Normal

If $S$ is also normal, then $SN$ is normal and the theorem becomes a special case of the Third Isomorphism Theorem.

### Case 3: $S \subseteq N$

If $S \subseteq N$, then $SN = N$ and $S \cap N = S$, so the theorem becomes the trivial statement $N/N \cong S/S$.

## Related Theorems

### First Isomorphism Theorem
Relates $G/\ker(\phi)$ to $\text{Im}(\phi)$ for homomorphisms $\phi: G \to H$.

### Third Isomorphism Theorem
Provides a "cancellation" rule for quotients: $(G/N)/(K/N) \cong G/K$.

## Summary

The Second Isomorphism Theorem is a powerful tool for understanding the relationships between subgroups, normal subgroups, and their quotients. It is particularly useful when working with products of subgroups and provides a bridge between different quotient constructions.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/First Isomorphism Theorem\|First Isomorphism Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Third Isomorphism Theorem\|Third Isomorphism Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Quotient Groups\|Quotient Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Subgroups\|Subgroups]] 