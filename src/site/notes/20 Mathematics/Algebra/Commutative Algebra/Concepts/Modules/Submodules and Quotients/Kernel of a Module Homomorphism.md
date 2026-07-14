---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Kernel of a Module Homomorphism/","title":"Kernel of a Module Homomorphism","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"],"dg-note-properties":{"title":"Kernel of a Module Homomorphism","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"]}}
---


# Kernel of a Module Homomorphism

For an $A$-linear map $f:M\to N$, the **kernel** is

$$\ker f=\{m\in M:f(m)=0\}.$$

It is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Submodule\|Submodule]] of $M$. The map $f$ is injective exactly when $\ker f=0$.

The kernel is the complete collection of relations erased by $f$. Quotienting them out gives an injective description of the reached part:

$$M/\ker f\cong\operatorname{im}f$$

by the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/First Isomorphism Theorem for Modules\|First Isomorphism Theorem for Modules]]. In an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Exact Sequences/Exact Sequence\|Exact Sequence]], exactness at $M$ says that the incoming [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Image of a Module Homomorphism\|image]] equals the outgoing kernel.

## Source

- `02_02_submodules_and_quotient_modules.pdf`, printed pp. 18-19.
