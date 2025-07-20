---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups/"}
---


# Normal Subgroups

## Introduction

The set of cosets of a subgroup raises a natural question: can this set itself be endowed with a group structure? This leads to the concept of normal subgroups, which are essential for constructing quotient groups.

## Definition

**Definition 2.3**: A subgroup $N$ of a group $G$ is a **normal subgroup** if for every $g \in G$, $gNg^{-1} = N$. This is denoted by $N \trianglelefteq G$.

The condition $gNg^{-1} = N$ is equivalent to $gN = Ng$ for all $g \in G$.

## Equivalent Characterizations

A subgroup $N$ of $G$ is normal if and only if any of the following conditions hold:

1. **Conjugation condition**: $gNg^{-1} = N$ for all $g \in G$
2. **Coset condition**: $gN = Ng$ for all $g \in G$
3. **Kernel condition**: $N$ is the kernel of some homomorphism from $G$ to another group
4. **Invariance condition**: $N$ is invariant under all inner automorphisms of $G$

## Examples

### Example 1: Normal Subgroups in Abelian Groups

In an abelian group, every subgroup is normal because $gng^{-1} = n$ for all $g, n \in G$.

**Examples**:
- In $(\mathbb{Z}, +)$, every subgroup $n\mathbb{Z}$ is normal
- In $(\mathbb{Q}^*, \cdot)$, the subgroup $\{1, -1\}$ is normal

### Example 2: Normal Subgroups in $D_4$

Consider the subgroup $N = \{e, r^2\}$ in $D_4$:
- For any rotation $r^k$: $r^k N = N r^k$ (since $r^2$ commutes with rotations)
- For any reflection $sr^k$: $(sr^k)N = N(sr^k)$ (since $r^2$ is in the center)

Therefore, $N$ is normal, and $D_4/N$ is a group of order 4.

### Example 3: The Alternating Group

The alternating group $A_n$ is a normal subgroup of the symmetric group $S_n$ because:
- $A_n$ is the kernel of the sign homomorphism $\text{sgn}: S_n \to \{\pm 1\}$
- The quotient group $S_n/A_n$ is isomorphic to $\{\pm 1\}$

### Example 4: Center of a Group

The center $Z(G)$ of a group $G$ is always a normal subgroup because:
- $Z(G) = \{z \in G \mid gz = zg \text{ for all } g \in G\}$
- For any $g \in G$ and $z \in Z(G)$: $gzg^{-1} = z \in Z(G)$

## Properties

### Intersection of Normal Subgroups
The intersection of any collection of normal subgroups is itself a normal subgroup.

### Product of Normal Subgroups
If $N$ and $M$ are normal subgroups of $G$, then $NM = MN$ is also a normal subgroup of $G$.

### Subgroup of Index 2
Any subgroup of index 2 is normal.

**Proof**: If $[G : H] = 2$, then there are exactly two left cosets: $H$ and $gH$ for some $g \notin H$. Similarly, there are exactly two right cosets: $H$ and $Hg'$ for some $g' \notin H$. Since $gH \cup H = G = H \cup Hg'$, we must have $gH = Hg'$, which implies $H$ is normal.

## Non-Normal Subgroups

### Example 1: Subgroups in $S_3$

Consider the subgroup $H = \{e, (1,2)\}$ in $S_3$:
- $(1,3)H = \{(1,3), (1,2,3)\}$
- $H(1,3) = \{(1,3), (1,3,2)\}$
- Since $(1,3)H \neq H(1,3)$, $H$ is not normal

### Example 2: Subgroups in $D_4$

Consider the subgroup $H = \{e, s\}$ in $D_4$:
- $rH = \{r, rs\} = \{r, sr^3\}$
- $Hr = \{r, sr\} = \{r, sr\}$
- Since $rH \neq Hr$, $H$ is not normal

## Applications

### Application 1: Quotient Groups
Normal subgroups are essential for constructing quotient groups, which are fundamental in group theory.

### Application 2: Homomorphisms
Normal subgroups are precisely the kernels of group homomorphisms.

### Application 3: Group Structure
Normal subgroups help us understand the structure of groups through the isomorphism theorems.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Subgroups\|Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Cosets\|Cosets]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Quotient Groups\|Quotient Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Group Homomorphisms\|Group Homomorphisms]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Isomorphism Theorems\|Isomorphism Theorems]] 