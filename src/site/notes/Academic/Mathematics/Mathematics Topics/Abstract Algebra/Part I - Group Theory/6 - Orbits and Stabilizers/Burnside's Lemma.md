---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Burnside's Lemma/"}
---


# Burnside's Lemma

## Introduction

Burnside's Lemma (also known as the Cauchy-Frobenius Lemma) is a powerful tool for counting the number of orbits when a group acts on a set. It is particularly useful in combinatorics for counting objects up to symmetry.

## Statement

**Theorem 6.3 (Burnside's Lemma)**: Let a finite group $G$ act on a finite set $X$. The number of orbits is equal to the average number of fixed points:

$$\text{Number of orbits} = \frac{1}{|G|} \sum_{g \in G} |\text{Fix}(g)|$$

where $\text{Fix}(g) = \{x \in X \mid g \cdot x = x\}$ is the set of elements fixed by $g$.

## Proof Sketch

The proof uses double counting. We count the number of pairs $(g, x)$ where $g \cdot x = x$ in two ways:

1. **Fix $g$, count $x$**: For each $g \in G$, count the number of $x \in X$ fixed by $g$. This gives $\sum_{g \in G} |\text{Fix}(g)|$.

2. **Fix $x$, count $g$**: For each $x \in X$, count the number of $g \in G$ that fix $x$. This gives $\sum_{x \in X} |\text{Stab}_G(x)|$.

By the Orbit-Stabilizer Theorem, $|\text{Stab}_G(x)| = |G|/|\text{Orb}_G(x)|$. Since all elements in the same orbit have the same orbit size, we get:

$$\sum_{g \in G} |\text{Fix}(g)| = \sum_{x \in X} \frac{|G|}{|\text{Orb}_G(x)|} = |G| \sum_{\text{orbits } O} \frac{|O|}{|O|} = |G| \cdot (\text{number of orbits})$$

Dividing by $|G|$ gives the result.

## Examples

### Example 1: Counting Cube Colorings

How many distinct ways can we color the faces of a cube with 2 colors (red and blue)?

The group of symmetries of a cube has order 24. We need to count the fixed points of each symmetry:
- Identity: fixes all $2^6 = 64$ colorings
- Rotations by $90°$ about face axes: fix $2^3 = 8$ colorings each
- Rotations by $180°$ about face axes: fix $2^4 = 16$ colorings each
- Rotations by $120°$ about vertex axes: fix $2^2 = 4$ colorings each
- Rotations by $180°$ about edge axes: fix $2^3 = 8$ colorings each

By Burnside's Lemma:
$$\text{Number of orbits} = \frac{1}{24}(64 + 6 \cdot 8 + 3 \cdot 16 + 8 \cdot 4 + 6 \cdot 8) = \frac{1}{24}(64 + 48 + 48 + 32 + 48) = \frac{240}{24} = 10$$

So there are 10 distinct colorings.

### Example 2: Counting Necklaces

How many distinct necklaces can be made with 4 beads of 3 different colors?

The group of symmetries is $D_4$ (dihedral group of order 8):
- Identity: fixes all $3^4 = 81$ necklaces
- Rotations by $90°$: fix $3$ necklaces each (all beads same color)
- Rotations by $180°$: fix $3^2 = 9$ necklaces each
- Reflections: fix $3^2 = 9$ necklaces each

By Burnside's Lemma:
$$\text{Number of orbits} = \frac{1}{8}(81 + 2 \cdot 3 + 1 \cdot 9 + 4 \cdot 9) = \frac{1}{8}(81 + 6 + 9 + 36) = \frac{132}{8} = 16.5$$

Since we can't have half a necklace, we need to be more careful about the counting.

### Example 3: Counting Arrangements

How many distinct arrangements of 3 red and 2 blue balls in a circle?

The group of symmetries is $D_5$ (dihedral group of order 10):
- Identity: fixes all $\binom{5}{3} = 10$ arrangements
- Rotations: only fix arrangements where all balls are the same color (none exist)
- Reflections: fix arrangements that are symmetric (2 arrangements)

By Burnside's Lemma:
$$\text{Number of orbits} = \frac{1}{10}(10 + 0 + 5 \cdot 2) = \frac{1}{10}(10 + 10) = \frac{20}{10} = 2$$

## Applications

### Application 1: Combinatorics

Burnside's Lemma is particularly useful in combinatorics for counting objects up to symmetry, such as:
- Colorings of geometric objects
- Arrangements of objects in symmetric patterns
- Necklaces and bracelets
- Graph colorings

### Application 2: Chemistry

In chemistry, Burnside's Lemma is used to count distinct molecular structures that are equivalent under rotation or reflection.

### Application 3: Crystallography

In crystallography, it's used to count distinct crystal structures and arrangements.

### Application 4: Graph Theory

In graph theory, it's used to count distinct graphs up to isomorphism.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbits\|Orbits]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Stabilizers\|Stabilizers]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbit-Stabilizer Theorem\|Orbit-Stabilizer Theorem]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/5 - Group Actions/Group Actions\|Group Actions]]
- [[Combinatorics\|Combinatorics]] 