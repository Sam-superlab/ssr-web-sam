---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring/","dg-note-properties":{}}
---


# Ring

A **ring** $A$ in Atiyah and Macdonald is a set with addition and multiplication such that:

1. $(A,+)$ is an abelian group with identity $0$;
2. multiplication is associative;
3. multiplication distributes over addition;
4. multiplication is commutative;
5. there is an identity $1$ for multiplication.

The book allows $1=0$, giving the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Zero Ring\|Zero Ring]]. Unless stated otherwise, every occurrence of “ring” in these notes uses the same commutative, unital convention.

## Basic consequences

For all $a,b\in A$,

$$
a0=0,\qquad (-a)b=-(ab),\qquad (-a)(-b)=ab.
$$

The multiplicative identity is unique. A ring can still have [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/03 Zero Divisors Nilpotents and Units/Zero Divisor\|zero divisors]], [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/03 Zero Divisors Nilpotents and Units/Nilpotent Element\|nilpotents]], and nonzero elements that are not [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/03 Zero Divisors Nilpotents and Units/Unit\|units]].

## Examples and nonexamples

- $\mathbb Z$, $\mathbb Z/n\mathbb Z$, every [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/03 Zero Divisors Nilpotents and Units/Field\|Field]], and polynomial rings $k[x_1,\ldots,x_n]$ are rings.
- The integers under usual addition but with multiplication $a*b=0$ have no multiplicative identity unless the ring is trivial, so they are not a ring in this convention.
- Matrix rings $M_n(k)$ for $n>1$ are not commutative, so they fall outside the book's standing convention even though they are rings in a broader sense.

## Related concepts

Structure-preserving maps are [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring Homomorphism\|ring homomorphisms]]. Additively closed, absorbent subsets are [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Ideal\|ideals]], and these are exactly the subsets by which one may form [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Quotient Ring\|quotient rings]].

## Source

- 01_01_rings_and_ring_homomorphisms.pdf, printed p. 1 (ring axioms and convention).

