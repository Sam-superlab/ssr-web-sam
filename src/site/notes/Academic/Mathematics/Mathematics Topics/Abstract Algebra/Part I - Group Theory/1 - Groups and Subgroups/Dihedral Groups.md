---
dg-publish: true
---

# Dihedral Groups

## Introduction

The dihedral groups are among the simplest and most important examples of finite, non-abelian groups. They are the symmetry groups of regular polygons and provide excellent examples for understanding group theory concepts.

## Definition

### Geometric Definition
The **dihedral group** $D_n$ is the group of symmetries of a regular $n$-gon. For $n \geq 3$, this group consists of:
- $n$ rotational symmetries
- $n$ reflectional symmetries

The order of $D_n$ is $2n$.

### Algebraic Presentation
The structure of $D_n$ can be captured by two generators: a rotation $r$ and a reflection $s$. The group is defined by the relations these generators satisfy:

$$D_n = \langle r, s \mid r^n = s^2 = e, \text{ and } srs^{-1} = r^{-1} \rangle$$

The relation $srs^{-1} = r^{-1}$ (or equivalently, $sr = r^{-1}s$) algebraically encodes the geometric fact that reflecting a rotation is equivalent to rotating in the opposite direction.

## Structure

### Elements
The elements of $D_n$ can be written as:
- **Rotations**: $\{e, r, r^2, \ldots, r^{n-1}\}$
- **Reflections**: $\{s, sr, sr^2, \ldots, sr^{n-1}\}$

### Group Operation
The group operation is function composition, which is not commutative. For example, a rotation by $90°$ followed by a horizontal flip $(sr)$ is not the same as a horizontal flip followed by a $90°$ rotation $(rs)$.

## Examples

### Example 1: The Group $D_4$ (Square)

The group $D_4$ represents the symmetries of a square and has order $2 \times 4 = 8$. Its elements are:

**Four rotations**:
- $e$: identity (rotation by $0°$)
- $r$: rotation by $90°$ counterclockwise
- $r^2$: rotation by $180°$ counterclockwise
- $r^3$: rotation by $270°$ counterclockwise

**Four reflections**:
- $s$: reflection across the horizontal axis
- $sr$: reflection across the main diagonal
- $sr^2$: reflection across the vertical axis
- $sr^3$: reflection across the anti-diagonal

### Example 2: The Group $D_3$ (Triangle)

The group $D_3$ represents the symmetries of an equilateral triangle and has order $2 \times 3 = 6$. Its elements are:

**Three rotations**:
- $e$: identity (rotation by $0°$)
- $r$: rotation by $120°$ counterclockwise
- $r^2$: rotation by $240°$ counterclockwise

**Three reflections**:
- $s$: reflection across the altitude from vertex 1
- $sr$: reflection across the altitude from vertex 2
- $sr^2$: reflection across the altitude from vertex 3

### Example 3: The Group $D_6$ (Hexagon)

The group $D_6$ has order 12 and represents the symmetries of a regular hexagon.

## Cayley Table

### Cayley Table for $D_4$

| $\cdot$ | $e$ | $r$ | $r^2$ | $r^3$ | $s$ | $sr$ | $sr^2$ | $sr^3$ |
|---------|-----|-----|-------|-------|-----|------|--------|--------|
| $e$     | $e$ | $r$ | $r^2$ | $r^3$ | $s$ | $sr$ | $sr^2$ | $sr^3$ |
| $r$     | $r$ | $r^2$ | $r^3$ | $e$ | $sr^3$ | $s$ | $sr$ | $sr^2$ |
| $r^2$   | $r^2$ | $r^3$ | $e$ | $r$ | $sr^2$ | $sr^3$ | $s$ | $sr$ |
| $r^3$   | $r^3$ | $e$ | $r$ | $r^2$ | $sr$ | $sr^2$ | $sr^3$ | $s$ |
| $s$     | $s$ | $sr$ | $sr^2$ | $sr^3$ | $e$ | $r$ | $r^2$ | $r^3$ |
| $sr$    | $sr$ | $sr^2$ | $sr^3$ | $s$ | $r^3$ | $e$ | $r$ | $r^2$ |
| $sr^2$  | $sr^2$ | $sr^3$ | $s$ | $sr$ | $r^2$ | $r^3$ | $e$ | $r$ |
| $sr^3$  | $sr^3$ | $s$ | $sr$ | $sr^2$ | $r$ | $r^2$ | $r^3$ | $e$ |

## Properties

### Non-abelian
Dihedral groups are non-abelian for $n \geq 3$. For example, in $D_4$:
- $rs = sr^3 \neq sr$

### Subgroups
The subgroups of $D_n$ include:
- The cyclic subgroup of rotations: $\{e, r, r^2, \ldots, r^{n-1}\}$
- Various reflection subgroups
- The trivial subgroup $\{e\}$

### Center
The center of $D_n$ is:
- $\{e\}$ if $n$ is odd
- $\{e, r^{n/2}\}$ if $n$ is even

## Applications

### Geometric Applications
- Study of crystal symmetries
- Analysis of molecular symmetries in chemistry
- Understanding tiling patterns

### Algebraic Applications
- Examples of non-abelian groups
- Understanding group presentations
- Study of group actions

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Group Axioms\|Group Axioms]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Subgroups\|Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Group Actions\|Group Actions]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Symmetric Groups\|Symmetric Groups]]
- [[Cyclic Groups\|Cyclic Groups]] 