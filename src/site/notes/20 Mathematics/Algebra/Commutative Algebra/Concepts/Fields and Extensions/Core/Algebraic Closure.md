---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Fields and Extensions/Core/Algebraic Closure/","title":"Algebraic Closure","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/fields-and-extensions"],"dg-note-properties":{"title":"Algebraic Closure","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/fields-and-extensions"],"aliases":["Algebraic Closure of a Field"]}}
---


# Algebraic Closure

An **algebraic closure** of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Field\|Field]] $K$ is an algebraic extension $\overline K/K$ such that $\overline K$ is algebraically closed. Equivalently, every nonconstant polynomial in $\overline K[t]$ splits into linear factors over $\overline K$.

## Existence and uniqueness

Every field has an algebraic closure. Any two algebraic closures of $K$ are isomorphic by an isomorphism that fixes $K$, but such an isomorphism is generally not canonical.

One existence proof is the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Fields and Extensions/Core/Artin Construction of an Algebraic Closure\|Artin Construction of an Algebraic Closure]], which repeatedly adjoins roots of all irreducible polynomials.

## Examples

- $\mathbb C$ is an algebraic closure of $\mathbb R$.
- The field of algebraic numbers inside $\mathbb C$ is an algebraic closure of $\mathbb Q$.
- An algebraically closed field is its own algebraic closure.

## Distinctions

An algebraic closure is an algebraic extension that is algebraically closed. An **algebraically closed extension** of $K$ need not be algebraic over $K$, so it need not be an algebraic closure.

## Source

- Standard field-theoretic definition; `01_08_exercises.pdf`, Exercise 13, supplies Artin's existence construction.
