---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Modules/Exactness of Localization/","title":"Exactness of Localization","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"],"dg-note-properties":{"title":"Exactness of Localization","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"],"aliases":["Localization Is Exact"]}}
---


# Exactness of Localization
The localization functor $M\mapsto S^{-1}M$ preserves every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Exact Sequences/Exact Sequence\|Exact Sequence]]. If

$$
M'\xrightarrow{f}M\xrightarrow{g}M''
$$

is exact at $M$, then its localization is exact at $S^{-1}M$.

## Mechanism

Suppose $g(m)/s=0$. Then some $t\in S$ kills $g(m)$, so $g(tm)=0$. Exactness gives $tm=f(m')$, and $m/s=f(m')/(st)$. The extra denominator converts eventual vanishing into an actual preimage.

## Consequences

- Localization preserves injections and surjections.
- $S^{-1}(M/N)\cong S^{-1}M/S^{-1}N$.
- It commutes with finite sums and finite intersections of submodules.
- $S^{-1}A$ is [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Flatness and Tor/Flat Module\|flat]] over $A$ because $S^{-1}M\cong S^{-1}A\otimes_A M$.

Localization need not commute with arbitrary infinite intersections; finiteness in the standard statement is meaningful.

## Source

- 03_00_rings_and_modules_of_fractions.pdf, A&M Proposition 3.3, Corollary 3.4, Proposition 3.5, and Corollary 3.6, printed pp. 39--40.
