---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.02 Submodules and Quotient Modules/Correspondence Theorem for Modules/","dg-note-properties":{}}
---


# Correspondence Theorem for Modules

Let $N$ be a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.02 Submodules and Quotient Modules/Submodule\|Submodule]] of an $A$-module $M$. There is an inclusion-preserving bijection

$$\{L\subseteq M:L\text{ is a submodule and }N\subseteq L\}$$
$$\longleftrightarrow$$
$$\{\overline L\subseteq M/N:\overline L\text{ is a submodule}\}.$$

It sends $L$ to $L/N$; the inverse sends a submodule of $M/N$ to its preimage under the quotient projection $M\to M/N$.

## Intuition

Once $N$ has been declared zero, every larger submodule $L$ leaves behind exactly the submodule $L/N$. Conversely, every submodule downstairs remembers a unique submodule upstairs containing all elements already collapsed by the quotient.

This correspondence preserves sums, intersections, and inclusions. It specializes to the familiar ideal correspondence for a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Quotient Ring\|Quotient Ring]].

## Source

- `02_02_submodules_and_quotient_modules.pdf`, printed p. 18.
