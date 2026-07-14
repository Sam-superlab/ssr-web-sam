---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Krull's Maximal Ideal Theorem/","title":"Krull's Maximal Ideal Theorem","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Krull's Maximal Ideal Theorem","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"aliases":["Maximal Ideal Theorem"]}}
---


# Krull's Maximal Ideal Theorem
Every nonzero [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] has at least one [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Maximal Ideal\|Maximal Ideal]]. More generally, every proper [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] $\mathfrak a\subsetneq A$ is contained in a maximal ideal.

## Proof idea

Consider the partially ordered set

$$
\Sigma=\{\mathfrak b\triangleleft A:\mathfrak a\subseteq\mathfrak b\subsetneq A\}
$$

ordered by inclusion. It is nonempty because it contains $\mathfrak a$.

For a chain $\{\mathfrak b_\lambda\}$ in $\Sigma$, the union

$$
\mathfrak b=\bigcup_\lambda\mathfrak b_\lambda
$$

is an ideal. The chain condition ensures that any two chosen elements lie together in one member, so their sum is still in the union. The union is proper: if $1$ belonged to it, then $1$ would already belong to some $\mathfrak b_\lambda$. Thus every chain has an upper bound, and Zorn's lemma supplies a maximal member of $\Sigma$.

Alternatively, the general statement follows by applying the nonzero-ring case to $A/\mathfrak a$ and using the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Correspondence Theorem for Ideals\|Correspondence Theorem for Ideals]].

## Corollary

Every nonunit belongs to a maximal ideal. If $x$ is not a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Unit\|Unit]], then $(x)$ is proper and hence lies in a maximal ideal. Conversely, no maximal ideal can contain a unit.

## Logical note

For arbitrary rings this theorem uses a form of the axiom of choice. In a Noetherian ring, ascending chains stabilize, so a maximal proper ideal can be obtained without a separate appeal to Zorn's lemma.

## Source

- 01_04_prime_and_maximal_ideals.pdf, printed pp. 3-4; Theorem 1.3 and Corollaries 1.4-1.5.

