---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Foundations/Faithful Module/","title":"Faithful Module","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"],"dg-note-properties":{"title":"Faithful Module","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"]}}
---


# Faithful Module

An $A$-module $M$ is **faithful** if

$$\operatorname{Ann}_A(M)=0.$$

Equivalently, whenever $aM=0$, one must have $a=0$. The action map

$$A\longrightarrow\operatorname{End}_{\mathbb Z}(M)$$

is then injective, so the module detects every scalar.

Every module becomes faithful after replacing $A$ by $A/\operatorname{Ann}_A(M)$. This changes the scalar ring but not the actual action on $M$.

## Examples

- The regular module $A$ is faithful.
- $A/I$ is usually not faithful as an $A$-module; its [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Foundations/Annihilator\|Annihilator]] is $I$. It is faithful as an $A/I$-module.

## Source

- `02_03_operations_on_submodules.pdf`, printed p. 20.
