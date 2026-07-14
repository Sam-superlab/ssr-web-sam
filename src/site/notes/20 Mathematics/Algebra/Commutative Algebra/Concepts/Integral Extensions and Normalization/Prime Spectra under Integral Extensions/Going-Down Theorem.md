---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Prime Spectra under Integral Extensions/Going-Down Theorem/","title":"Going-Down Theorem","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/integral-extensions-and-normalization"],"dg-note-properties":{"title":"Going-Down Theorem","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/integral-extensions-and-normalization"]}}
---


# Going-Down Theorem

Let $A\subseteq B$ be integral domains, with $A$ an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Integral Closure and Normality/Integrally Closed Domain\|Integrally Closed Domain]] and $B$ integral over $A$. Given a descending chain

$$
\mathfrak p_1\supseteq\cdots\supseteq\mathfrak p_n
$$

and a compatible partial descending chain of primes in $B$, the chain upstairs can be extended downward so that each prime contracts to the corresponding $\mathfrak p_i$.

## One-step idea

Given $\mathfrak p_1\supseteq\mathfrak p_2$ and $\mathfrak q_1$ over $\mathfrak p_1$, one seeks a prime $\mathfrak q_2\subseteq\mathfrak q_1$ over $\mathfrak p_2$. By the prime-contraction criterion, it is enough to establish the right contraction after localizing $B$ at $\mathfrak q_1$ and extending $\mathfrak p_2$.

Minimal-polynomial coefficients of elements integral over $\mathfrak p_2$ lie in $\mathfrak p_2$. If an element of $A$ entered the contraction without lying in $\mathfrak p_2$, this coefficient control would force a denominator into $\mathfrak q_1$, a contradiction.

## Hypotheses matter

Unlike the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Integral Extensions and Normalization/Prime Spectra under Integral Extensions/Going-Up Theorem\|Going-Up Theorem]], going down is not asserted for arbitrary integral ring extensions. The domain and integrally closed assumptions are doing real work.

## Source

- 05_03_integrally_closed_going_down.pdf, A&M Theorem 5.16, printed p. 64.
