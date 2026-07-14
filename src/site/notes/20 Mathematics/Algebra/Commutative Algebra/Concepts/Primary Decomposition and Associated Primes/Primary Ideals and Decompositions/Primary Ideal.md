---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Primary Decomposition and Associated Primes/Primary Ideals and Decompositions/Primary Ideal/","title":"Primary Ideal","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/primary-decomposition-and-associated-primes"],"dg-note-properties":{"title":"Primary Ideal","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/primary-decomposition-and-associated-primes"]}}
---


# Primary Ideal

A proper [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] $\mathfrak q\subsetneq A$ is **primary** when

$$
xy\in\mathfrak q
\quad\Longrightarrow\quad
x\in\mathfrak q\text{ or }y^n\in\mathfrak q
\text{ for some }n>0.
$$

Equivalently, $A/\mathfrak q$ is nonzero and every zero-divisor in it is nilpotent.

## Radical

$\sqrt{\mathfrak q}$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|Prime Ideal]], the smallest prime containing $\mathfrak q$. If $\sqrt{\mathfrak q}=\mathfrak p$, call $\mathfrak q$ **$\mathfrak p$-primary**.

## Examples and nonexamples

- Every prime ideal is primary.
- $(p^n)\subseteq\mathbb Z$ is $(p)$-primary.
- $(x,y^2)\subseteq k[x,y]$ is $(x,y)$-primary but is not a power of $(x,y)$.
- A prime power need not be primary when the prime is not maximal.
- If $\sqrt{\mathfrak a}$ is maximal, then $\mathfrak a$ is primary; in particular every power of a maximal ideal is primary.

## Colon behavior

If $\mathfrak q$ is $\mathfrak p$-primary and $x\notin\mathfrak q$, then $(\mathfrak q:x)$ is again $\mathfrak p$-primary. If $x\notin\mathfrak p$, then $(\mathfrak q:x)=\mathfrak q$.

## Source

- 04_00_primary_decomposition.pdf, A&M Propositions 4.1--4.2 and Lemma 4.4, printed pp. 50--52.
