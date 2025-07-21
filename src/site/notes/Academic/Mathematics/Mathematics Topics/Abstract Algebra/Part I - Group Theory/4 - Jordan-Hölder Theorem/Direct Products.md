---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/4 - Jordan-Hölder Theorem/Direct Products/"}
---


# Direct Products

## Introduction

While composition series break groups down, direct products build them up. Direct products allow us to construct larger groups from smaller ones and provide a powerful tool for understanding group structure.

## External Direct Product

**Definition 4.4 (External Direct Product)**: Given two groups $(G, *_G)$ and $(H, *_H)$, their **external direct product** $G \times H$ is the set of ordered pairs $\{(g,h) \mid g \in G, h \in H\}$ with the component-wise operation:

$$(g_1, h_1) \cdot (g_2, h_2) = (g_1 *_G g_2, h_1 *_H h_2)$$

This construction creates a new, larger group from $G$ and $H$. The order of the direct product is $|G \times H| = |G| \cdot |H|$.

## Internal Direct Product

Often, we want to recognize if a given group is isomorphic to a direct product of some of its subgroups.

**Theorem 4.5 (Internal Direct Product)**: Let $G$ be a group with subgroups $H$ and $K$. If:
1. $H$ and $K$ are normal subgroups of $G$
2. $G = HK$
3. $H \cap K = \{e\}$

then $G$ is isomorphic to the external direct product $H \times K$.

## Properties of Direct Products

### Order
The order of a direct product is the product of the orders: $|G \times H| = |G| \cdot |H|$.

### Cyclic Groups
An important property relates to the structure of cyclic groups. The direct product $\mathbb{Z}_m \times \mathbb{Z}_n$ is cyclic (and thus isomorphic to $\mathbb{Z}_{mn}$) if and only if $m$ and $n$ are relatively prime. This is a group-theoretic restatement of the Chinese Remainder Theorem.

### Abelian Groups
The direct product of abelian groups is abelian.

### Commutativity
Elements from different factors commute: $(g, e_H) \cdot (e_G, h) = (e_G, h) \cdot (g, e_H) = (g, h)$.

## Examples

### Example 1: Direct Product of Cyclic Groups

Consider $\mathbb{Z}_2 \times \mathbb{Z}_3$:
- Order: $2 \times 3 = 6$
- Since $\gcd(2, 3) = 1$, this group is cyclic and isomorphic to $\mathbb{Z}_6$
- Elements: $(0,0), (0,1), (0,2), (1,0), (1,1), (1,2)$

### Example 2: Direct Product Decomposition

Consider the group $\mathbb{Z}_6 \times \mathbb{Z}_{10}$. Since $\gcd(6, 10) = 2 \neq 1$, this group is not cyclic. However, we can decompose it as:

$$\mathbb{Z}_6 \times \mathbb{Z}_{10} \cong (\mathbb{Z}_2 \times \mathbb{Z}_3) \times (\mathbb{Z}_2 \times \mathbb{Z}_5) \cong \mathbb{Z}_2 \times \mathbb{Z}_2 \times \mathbb{Z}_3 \times \mathbb{Z}_5$$

### Example 3: Internal Direct Product

Consider the dihedral group $D_6$ (symmetries of a regular hexagon). Let $H = \langle r^2 \rangle$ (rotations by multiples of $120°$) and $K = \langle s \rangle$ (reflection across a fixed axis).

- $H$ and $K$ are normal subgroups
- $D_6 = HK$
- $H \cap K = \{e\}$

Therefore, $D_6 \cong H \times K \cong \mathbb{Z}_3 \times \mathbb{Z}_2 \cong \mathbb{Z}_6$.

### Example 4: Klein Four-Group

The Klein four-group $V$ can be written as:
$$V \cong \mathbb{Z}_2 \times \mathbb{Z}_2$$

This is the smallest non-cyclic group.

## Applications

### Application 1: Classification of Finite Abelian Groups

Direct products are fundamental to the classification of finite abelian groups, which states that every finite abelian group is isomorphic to a direct product of cyclic groups of prime power order.

### Application 2: Understanding Group Structure

Direct products allow us to build complex groups from simpler ones, providing insight into group structure.

### Application 3: Representation Theory

Direct products are important in representation theory, where they correspond to tensor products of representations.

### Application 4: Cryptography

Direct products are used in cryptography, particularly in the construction of cryptographic protocols based on group theory.

## Generalizations

### Direct Product of Multiple Groups

The direct product can be extended to any finite number of groups:
$$G_1 \times G_2 \times \cdots \times G_n$$

### Infinite Direct Products

For infinite families of groups, we can define the direct product as the set of all functions from the index set to the union of the groups, with component-wise operations.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Subgroups\|Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Cyclic Groups\|Cyclic Groups]]
- [[Abelian Groups\|Abelian Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/10 - Special Ideals and Domains/Chinese Remainder Theorem\|Chinese Remainder Theorem]] 