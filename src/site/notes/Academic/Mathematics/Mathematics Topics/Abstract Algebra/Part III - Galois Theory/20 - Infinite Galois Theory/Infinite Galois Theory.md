---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part III - Galois Theory/20 - Infinite Galois Theory/Infinite Galois Theory/"}
---


# Infinite Galois Theory

## Introduction

The powerful correspondence of Galois theory can be extended from finite to infinite algebraic extensions, but this requires the introduction of topological concepts. The fundamental theorem in its original form fails because there are "too many" subgroups of the Galois group to correspond bijectively with the intermediate fields.

## The Problem with Infinite Extensions

### Why the Original Theorem Fails

For an infinite Galois extension $L/K$, the Galois group $\text{Gal}(L/K)$ is also infinite. The fundamental theorem in its original form fails because there are "too many" subgroups of $\text{Gal}(L/K)$ to correspond bijectively with the intermediate fields.

### The Solution: Topology

The solution, introduced by Krull, is to define a topology on the Galois group, now called the **Krull topology**. In this topology, a basis of open neighborhoods of the identity is given by the subgroups $\text{Gal}(L/F)$ where $F$ is a finite extension of $K$ contained in $L$.

## The Krull Topology

### Definition

**Definition 20.1**: Let $L/K$ be a Galois extension. The **Krull topology** on $\text{Gal}(L/K)$ is defined by taking as a basis of open neighborhoods of the identity the subgroups $\text{Gal}(L/F)$ where $F$ is a finite extension of $K$ contained in $L$.

### Properties

With this structure, $\text{Gal}(L/K)$ becomes a **profinite group**—a topological group that is:
- Compact
- Hausdorff
- Totally disconnected

### Examples

**Example 1**: The Galois group of the algebraic closure $\overline{\mathbb{Q}}/\mathbb{Q}$ is a profinite group.

**Example 2**: The Galois group of the maximal abelian extension of $\mathbb{Q}$ is isomorphic to the profinite completion of $\mathbb{Z}$.

## The Fundamental Theorem for Infinite Extensions

**Theorem 20.2 (Fundamental Theorem of Infinite Galois Theory)**: Let $L/K$ be a Galois extension (possibly infinite). There is a one-to-one, inclusion-reversing correspondence between the intermediate fields of the extension and the **closed** subgroups of $\text{Gal}(L/K)$ (with the Krull topology).

### Key Differences from Finite Case

1. **Closed Subgroups**: Only closed subgroups correspond to intermediate fields
2. **Topological Structure**: The Galois group has a natural topology
3. **Compactness**: The Galois group is compact in the Krull topology

### Examples

**Example 1**: For the extension $\overline{\mathbb{Q}}/\mathbb{Q}$:
- The Galois group is the absolute Galois group of $\mathbb{Q}$
- The closed subgroups correspond to the intermediate fields
- Not all subgroups are closed

**Example 2**: For the maximal abelian extension of $\mathbb{Q}$:
- The Galois group is isomorphic to $\widehat{\mathbb{Z}}$
- The closed subgroups correspond to the abelian extensions of $\mathbb{Q}$

## Profinite Groups

### Definition

A **profinite group** is a topological group that is isomorphic to the inverse limit of a system of finite groups.

### Properties

- Profinite groups are compact, Hausdorff, and totally disconnected
- Every profinite group is the Galois group of some field extension
- The Krull topology makes the Galois group of any Galois extension profinite

### Examples

**Example 1**: The profinite completion of $\mathbb{Z}$ is isomorphic to $\prod_p \mathbb{Z}_p$ where the product is over all primes $p$.

**Example 2**: The absolute Galois group of a finite field is isomorphic to $\widehat{\mathbb{Z}}$.

## Applications

### Application 1: Class Field Theory

Infinite Galois theory is fundamental to class field theory, which describes the abelian extensions of number fields and local fields.

### Application 2: Galois Representations

The study of continuous representations of profinite Galois groups is central to modern number theory, particularly in the Langlands program.

### Application 3: Algebraic Geometry

Infinite Galois theory has applications in algebraic geometry, particularly in the study of étale fundamental groups.

## Examples

### Example 1: The Absolute Galois Group of $\mathbb{Q}$

The absolute Galois group $\text{Gal}(\overline{\mathbb{Q}}/\mathbb{Q})$ is one of the most important profinite groups in mathematics. It encodes information about all finite extensions of $\mathbb{Q}$.

### Example 2: The Maximal Abelian Extension

The Galois group of the maximal abelian extension of $\mathbb{Q}$ is isomorphic to $\widehat{\mathbb{Z}}^\times$, the group of units in the profinite completion of $\mathbb{Z}$.

### Example 3: Local Fields

For a local field $K$ (like $\mathbb{Q}_p$), the absolute Galois group has a particularly nice structure related to the ramification theory of the field.

## Advanced Topics

### Galois Cohomology

The study of continuous cohomology of profinite Galois groups is a powerful tool in number theory and algebraic geometry.

### Galois Representations

Continuous representations of profinite Galois groups into linear groups are fundamental to modern number theory.

### The Langlands Program

The Langlands program seeks to understand the relationship between Galois representations and automorphic representations, using infinite Galois theory as a key tool.

## Summary

Infinite Galois theory beautifully restores the Galois correspondence for the infinite case by restricting attention to the topologically significant (closed) subgroups. The introduction of topology provides the right framework for understanding infinite extensions.

This theory has profound applications throughout mathematics, from number theory to algebraic geometry to representation theory. The study of profinite groups and their representations continues to be an active area of research with connections to many other areas of mathematics. 