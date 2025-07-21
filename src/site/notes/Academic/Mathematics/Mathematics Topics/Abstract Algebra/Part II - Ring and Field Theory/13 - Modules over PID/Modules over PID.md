---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/13 - Modules over PID/Modules over PID/"}
---


# Modules over a PID

## Introduction

The concept of a module generalizes the notion of a vector space by allowing the "scalars" to come from a ring instead of a field. A module is to a ring what a vector space is to a field, making it a central, unifying concept in algebra.

## Definition and Basic Properties

### Definition

**Definition 13.1**: Let $R$ be a ring. A **left $R$-module** is an abelian group $(M, +)$ together with an operation $R \times M \to M$ (scalar multiplication) that satisfies certain compatibility axioms:

1. **Distributivity**: $r(m_1 + m_2) = rm_1 + rm_2$ for all $r \in R$, $m_1, m_2 \in M$
2. **Distributivity**: $(r_1 + r_2)m = r_1m + r_2m$ for all $r_1, r_2 \in R$, $m \in M$
3. **Associativity**: $(r_1r_2)m = r_1(r_2m)$ for all $r_1, r_2 \in R$, $m \in M$
4. **Identity**: $1 \cdot m = m$ for all $m \in M$ (if $R$ has a multiplicative identity)

### Examples

- **Vector Spaces**: If $R$ is a field, then an $R$-module is exactly a vector space over $R$
- **Abelian Groups**: Any abelian group is a $\mathbb{Z}$-module
- **Ideal Modules**: Any ideal $I$ of a ring $R$ is an $R$-module
- **Quotient Modules**: If $M$ is an $R$-module and $N$ is a submodule, then $M/N$ is an $R$-module

## Structure Theory for Modules over PIDs

The study of modules over arbitrary rings is vast and complex. However, when the ring of scalars is a PID, the structure of finitely generated modules can be completely and beautifully classified.

### Fundamental Theorem

**Theorem 13.2 (Fundamental Theorem of Finitely Generated Modules over a PID)**: Let $R$ be a PID and let $M$ be a finitely generated $R$-module. Then $M$ is isomorphic to a direct sum of the form:

$$M \cong R^f \oplus \frac{R}{(d_1)} \oplus \frac{R}{(d_2)} \oplus \cdots \oplus \frac{R}{(d_k)}$$

where $f \geq 0$ is an integer, and the $(d_i)$ are proper ideals of $R$ such that $d_1 \mid d_2 \mid \cdots \mid d_k$. The integer $f$ (the **free rank**) and the ideals $(d_i)$ (the **invariant factors**) are uniquely determined by $M$.

### Alternative Decomposition

An alternative decomposition, the **primary decomposition**, states that $M$ is isomorphic to:

$$M \cong R^f \oplus \frac{R}{(p_1^{r_1})} \oplus \frac{R}{(p_2^{r_2})} \oplus \cdots \oplus \frac{R}{(p_s^{r_s})}$$

where the $p_i$ are prime elements of $R$. The ideals $(p_i^{r_i})$ are called the **elementary divisors** and are also uniquely determined by $M$.

## Applications

This theorem is a powerful result with profound consequences, as it provides a unified framework for several key theorems in algebra:

### Application 1: Fundamental Theorem of Finitely Generated Abelian Groups

If we take the ring to be $R = \mathbb{Z}$ (which is a PID), an abelian group is simply a $\mathbb{Z}$-module. The theorem then gives a complete classification of all finitely generated abelian groups as direct products of cyclic groups.

**Corollary 13.3**: Every finitely generated abelian group is isomorphic to a direct sum of the form:

$$\mathbb{Z}^f \oplus \mathbb{Z}_{d_1} \oplus \mathbb{Z}_{d_2} \oplus \cdots \oplus \mathbb{Z}_{d_k}$$

where $f \geq 0$ and $d_1 \mid d_2 \mid \cdots \mid d_k$.

### Application 2: Jordan Canonical Form

Let $V$ be a finite-dimensional vector space over an algebraically closed field $F$, and let $T: V \to V$ be a linear transformation. We can turn $V$ into a module over the polynomial ring $F[x]$ (a PID) by defining $p(x) \cdot v = p(T)(v)$.

The structure theorem for this module then gives a decomposition of $V$ that corresponds to the Jordan Canonical Form of the matrix of $T$. The elementary divisors are of the form $(x - \lambda)^k$, which correspond directly to the Jordan blocks of the matrix.

### Application 3: Smith Normal Form

The structure theorem for modules over PIDs is closely related to the Smith normal form of matrices. Given a matrix $A$ over a PID $R$, there exist invertible matrices $P$ and $Q$ such that $PAQ$ is in Smith normal form (diagonal with each diagonal element dividing the next).

## Examples

### Example 1: Abelian Groups

Consider the abelian group $G = \mathbb{Z}_{12} \oplus \mathbb{Z}_{18}$. To find its structure, we need to find the invariant factors.

First, we find the prime power decomposition:
- $\mathbb{Z}_{12} \cong \mathbb{Z}_4 \oplus \mathbb{Z}_3$
- $\mathbb{Z}_{18} \cong \mathbb{Z}_2 \oplus \mathbb{Z}_9$

So $G \cong \mathbb{Z}_4 \oplus \mathbb{Z}_3 \oplus \mathbb{Z}_2 \oplus \mathbb{Z}_9$.

Now we group by primes:
- Powers of 2: $\mathbb{Z}_4 \oplus \mathbb{Z}_2 \cong \mathbb{Z}_4 \oplus \mathbb{Z}_2$
- Powers of 3: $\mathbb{Z}_3 \oplus \mathbb{Z}_9 \cong \mathbb{Z}_9 \oplus \mathbb{Z}_3$

The invariant factors are the least common multiples: $d_1 = 2$, $d_2 = 36$. So $G \cong \mathbb{Z}_2 \oplus \mathbb{Z}_{36}$.

### Example 2: Vector Space with Linear Transformation

Let $V = \mathbb{R}^3$ and let $T: V \to V$ be the linear transformation with matrix:

$$A = \begin{pmatrix} 2 & 1 & 0 \\ 0 & 2 & 1 \\ 0 & 0 & 2 \end{pmatrix}$$

We can view $V$ as an $\mathbb{R}[x]$-module where $x \cdot v = T(v)$. The characteristic polynomial is $(x - 2)^3$, and the minimal polynomial is also $(x - 2)^3$.

The elementary divisors are $(x - 2)^3$, so the Jordan canonical form has one Jordan block of size 3 with eigenvalue 2.

### Example 3: Module over $\mathbb{Z}[i]$

Consider the module $M = \mathbb{Z}[i]^2$ over the ring of Gaussian integers $\mathbb{Z}[i]$. Since $\mathbb{Z}[i]$ is a PID, any finitely generated submodule of $M$ will have a well-defined structure.

## Submodules and Quotient Modules

### Submodules

A **submodule** of an $R$-module $M$ is a subset $N \subseteq M$ that is closed under addition and scalar multiplication. Submodules are the analogues of subspaces in vector spaces.

### Quotient Modules

If $N$ is a submodule of $M$, then the quotient group $M/N$ can be made into an $R$-module by defining $r(m + N) = rm + N$.

### Isomorphism Theorems

The isomorphism theorems for groups have analogues for modules:

1. **First Isomorphism Theorem**: If $\phi: M \to N$ is a module homomorphism, then $M/\ker(\phi) \cong \text{im}(\phi)$
2. **Second Isomorphism Theorem**: If $N$ and $P$ are submodules of $M$, then $(N + P)/P \cong N/(N \cap P)$
3. **Third Isomorphism Theorem**: If $N \subseteq P \subseteq M$ are submodules, then $(M/N)/(P/N) \cong M/P$

## Free Modules

### Definition

An $R$-module $M$ is **free** if it has a basis, i.e., a linearly independent spanning set. Free modules are the analogues of vector spaces.

### Properties

- Every free module over a PID is isomorphic to $R^n$ for some $n$
- The rank of a free module is well-defined (unlike for general rings)
- Every submodule of a free module over a PID is free

## Torsion Modules

### Definition

An element $m$ of an $R$-module $M$ is a **torsion element** if there exists a non-zero $r \in R$ such that $rm = 0$. The set of all torsion elements forms a submodule called the **torsion submodule**.

### Structure

For modules over PIDs, the torsion submodule has a particularly nice structure, and every finitely generated module is the direct sum of its torsion submodule and a free module.

## Summary

Modules over PIDs provide a powerful framework for understanding the structure of many important algebraic objects. The fundamental theorem gives a complete classification of finitely generated modules, which unifies several key results in algebra.

This theory has applications throughout mathematics, from group theory to linear algebra to algebraic number theory. The study of modules continues to be an active area of research, with connections to many other areas of mathematics including representation theory, homological algebra, and algebraic geometry. 