---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Correspondence Theorem for Modules/","title":"Correspondence Theorem for Modules","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"],"dg-note-properties":{"title":"Correspondence Theorem for Modules","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"]}}
---


# Correspondence Theorem for Modules

Let $N$ be a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Submodule\|Submodule]] of an $A$-module $M$. There is an inclusion-preserving bijection

$$\{L\subseteq M:L\text{ is a submodule and }N\subseteq L\}$$
$$\longleftrightarrow$$
$$\{\overline L\subseteq M/N:\overline L\text{ is a submodule}\}.$$

It sends $L$ to $L/N$; the inverse sends a submodule of $M/N$ to its preimage under the quotient projection $M\to M/N$.

## Intuition

Once $N$ has been declared zero, every larger submodule $L$ leaves behind exactly the submodule $L/N$. Conversely, every submodule downstairs remembers a unique submodule upstairs containing all elements already collapsed by the quotient.

This correspondence preserves sums, intersections, and inclusions. It specializes to the familiar ideal correspondence for a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Quotient Ring\|Quotient Ring]].

## Source

- `02_02_submodules_and_quotient_modules.pdf`, printed p. 18.
