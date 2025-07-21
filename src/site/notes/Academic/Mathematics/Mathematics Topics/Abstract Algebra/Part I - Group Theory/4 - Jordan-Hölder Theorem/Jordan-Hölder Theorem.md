---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/4 - Jordan-Hölder Theorem/Jordan-Hölder Theorem/"}
---


# Jordan-Hölder Theorem

## Introduction

Having established that finite groups can be broken down into simple components, a crucial question remains: is this decomposition unique? The Jordan-Hölder theorem provides a resounding affirmative answer, solidifying the analogy with prime factorization.

## Statement

**Theorem 4.1 (Jordan-Hölder)**: Any two composition series of a given finite group have the same length. Furthermore, the sets of composition factors are isomorphic, up to a permutation of their order.

## Significance

This profound result guarantees that the simple "building blocks" of any finite group are an intrinsic property of that group, independent of the specific way it is decomposed. The set of simple groups that appear in a composition series is a fundamental invariant, much like the set of prime factors of an integer.

## Analogy with Prime Factorization

Just as every integer has a unique prime factorization (up to order), every finite group has a unique "simple group factorization" (up to order and isomorphism). This analogy provides the entire motivation for the classification of all finite simple groups.

## Examples

### Example 1: Composition Series of $\mathbb{Z}_{12}$

A composition series for $\mathbb{Z}_{12}$ is:
$$\{0\} \trianglelefteq \langle 6 \rangle \trianglelefteq \langle 2 \rangle \trianglelefteq \mathbb{Z}_{12}$$

The factors are:
- $\langle 6 \rangle / \{0\} \cong \mathbb{Z}_2$
- $\langle 2 \rangle / \langle 6 \rangle \cong \mathbb{Z}_3$
- $\mathbb{Z}_{12} / \langle 2 \rangle \cong \mathbb{Z}_2$

By the Jordan-Hölder theorem, any other composition series will have the same factors (up to isomorphism and order).

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

Any other composition series will have the same three factors of order 2.

## Applications

### Application 1: Classification of Finite Abelian Groups

The Jordan-Hölder theorem, combined with the fundamental theorem of finitely generated abelian groups, provides a complete classification of finite abelian groups up to isomorphism.

### Application 2: Understanding Group Structure

The theorem ensures that the decomposition into simple factors is unique, providing a powerful tool for understanding group structure.

### Application 3: Group Classification

The Jordan-Hölder theorem is fundamental to the classification of finite simple groups, one of the major achievements of 20th-century mathematics.

### Application 4: Solvability

The theorem helps determine whether a group is solvable by examining its composition factors. A group is solvable if and only if all its composition factors are abelian.

## Proof Strategy

The proof of the Jordan-Hölder theorem involves:

1. **Refinement**: Showing that any two subnormal series can be refined to have the same factors
2. **Schreier's Refinement Theorem**: Establishing that any two subnormal series have equivalent refinements
3. **Zassenhaus Lemma**: A technical lemma about the relationship between subgroups and normal subgroups

## Historical Context

The Jordan-Hölder theorem was first proved by Camille Jordan in 1869 and later refined by Otto Hölder in 1889. It represents one of the foundational results in group theory and provides the theoretical basis for the classification of finite simple groups.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Composition Series\|Composition Series]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Simple Groups\|Simple Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Normal Subgroups\|Normal Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/2 - Cosets and Lagrange's Theorem/Quotient Groups\|Quotient Groups]]
- [[Classification of Finite Simple Groups\|Classification of Finite Simple Groups]] 