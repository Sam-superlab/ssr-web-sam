---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.02 Submodules and Quotient Modules/Quotient Module/","dg-note-properties":{}}
---


# Quotient Module

If $N$ is a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.02 Submodules and Quotient Modules/Submodule\|Submodule]] of an $A$-module $M$, the **quotient module** $M/N$ is the quotient abelian group with scalar action

$$a(m+N)=am+N.$$

This is well-defined because replacing $m$ by $m+n$ changes $am$ by $an\in N$.

## Universal viewpoint

The projection $\pi:M\to M/N$ sends $N$ to zero. Every [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.01 Modules and Module Homomorphisms/Module Homomorphism\|Module Homomorphism]] $f:M\to P$ satisfying $N\subseteq\ker f$ factors uniquely as

$$M\xrightarrow{\pi}M/N\xrightarrow{\bar f}P.$$

Thus $M/N$ is the most general module obtained from $M$ by forcing every element of $N$ to vanish.

## Example

For an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Ideal\|Ideal]] $I\subseteq A$, the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Quotient Ring\|Quotient Ring]] $A/I$ is also the quotient of the $A$-module $A$ by its submodule $I$.

## Related

[[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.02 Submodules and Quotient Modules/First Isomorphism Theorem for Modules\|First Isomorphism Theorem for Modules]], [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.02 Submodules and Quotient Modules/Cokernel\|Cokernel]], [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.06 Exact Sequences/Short Exact Sequence\|Short Exact Sequence]].

## Source

- `02_02_submodules_and_quotient_modules.pdf`, printed pp. 18-19.
