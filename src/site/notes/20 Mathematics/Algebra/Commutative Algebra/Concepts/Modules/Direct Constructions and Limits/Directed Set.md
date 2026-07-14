---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Direct Constructions and Limits/Directed Set/","title":"Directed Set","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"],"dg-note-properties":{"title":"Directed Set","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"]}}
---


# Directed Set

A partially ordered set $I$ is **directed** if for every $i,j\in I$ there is some $k\in I$ with

$$i\le k\qquad\text{and}\qquad j\le k.$$

The point is not that any two indices are comparable, but that they admit a common later stage.

## Examples

- $\mathbb N$ with its usual order.
- Finite subsets of a set, ordered by inclusion; the union gives a common upper bound.
- Finitely generated submodules of a module, ordered by inclusion; the sum of two is a common upper bound.

Directed sets provide the index shapes for [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Direct Constructions and Limits/Direct System\|direct systems]] and [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Direct Constructions and Limits/Direct Limit\|direct limits]], where information is repeatedly mapped into later stages.

## Nonexample

Two incomparable maximal elements with no larger element form a poset that is not directed.

## Source

- `02_12_exercises.pdf`, printed p. 32; Exercise 14.
