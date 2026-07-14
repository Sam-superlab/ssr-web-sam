---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Algebras over Rings/Core/Algebra of Finite Type/","title":"Algebra of Finite Type","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/algebras-over-rings"],"dg-note-properties":{"title":"Algebra of Finite Type","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/algebras-over-rings"]}}
---


# Algebra of Finite Type

An $A$-algebra $B$ is **of finite type** if there exist $b_1,\ldots,b_n\in B$ such that

$$B=A[b_1,\ldots,b_n].$$

Equivalently, the evaluation map

$$A[t_1,\ldots,t_n]\twoheadrightarrow B,\qquad t_i\mapsto b_i,$$

is a surjective [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Algebras over Rings/Core/Algebra Homomorphism\|Algebra Homomorphism]].

Finite type means finitely many algebra generators; arbitrary polynomial expressions in them are allowed. This is weaker than being a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Algebras over Rings/Core/Module-Finite Algebra\|Module-Finite Algebra]], which requires finitely many $A$-module generators.

## Examples

- $A[x_1,\ldots,x_n]/I$ is of finite type over $A$.
- $A[x]$ is of finite type but generally not finite over $A$.
- A ring is called finitely generated, without naming a base, when it is of finite type as a $\mathbb Z$-algebra.

## Source

- `02_10_algebras.pdf`, printed p. 30.
