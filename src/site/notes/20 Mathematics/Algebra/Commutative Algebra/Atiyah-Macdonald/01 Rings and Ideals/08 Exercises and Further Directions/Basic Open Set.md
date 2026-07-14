---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/08 Exercises and Further Directions/Basic Open Set/","dg-note-properties":{}}
---


# Basic Open Set

For $f$ in a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring\|Ring]] $A$, the **basic open set**

$$
D(f)
=
\{\mathfrak p\in\operatorname{Spec}(A):f\notin\mathfrak p\}
$$

is the complement of $V(f)$ in the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/08 Exercises and Further Directions/Prime Spectrum\|Prime Spectrum]]. A&M writes this set as $X_f$.

The sets $D(f)$ form a basis for the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/08 Exercises and Further Directions/Zariski Topology\|Zariski Topology]].

## Identities

$$
D(f)\cap D(g)=D(fg),
$$

$$
D(f)=\varnothing
\iff
f\text{ is [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/03 Zero Divisors Nilpotents and Units/Nilpotent Element\|nilpotent]]},
$$

$$
D(f)=\operatorname{Spec}(A)
\iff
f\text{ is a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/03 Zero Divisors Nilpotents and Units/Unit\|Unit]]}.
$$

Also,

$$
D(f)=D(g)
\iff
\sqrt{(f)}=\sqrt{(g)}.
$$

## Quasi-compactness

Every basic open $D(f)$ is quasi-compact. In particular, $\operatorname{Spec}(A)=D(1)$ is quasi-compact.

The algebraic reason is finite generation of the unit ideal. If basic opens $D(f_i)$ cover the spectrum, then no prime contains all $f_i$, so the ideal they generate is $(1)$. Thus

$$
1=\sum_{i\in F}a_if_i
$$

for some finite subset $F$, and the corresponding finite collection still covers.

An open subset of $\operatorname{Spec}(A)$ is quasi-compact exactly when it is a finite union of basic opens.

## Source

- 01_08_exercises.pdf, printed p. 12; Exercise 17.

