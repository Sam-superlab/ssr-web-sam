---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.01 Modules and Module Homomorphisms/Hom Module/","dg-note-properties":{}}
---


# Hom Module

For $A$-modules $M,N$, the **Hom module**

$$\operatorname{Hom}_A(M,N)$$

is the set of all [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.01 Modules and Module Homomorphisms/Module Homomorphism\|$A$-linear maps]] $M\to N$, with pointwise addition and scalar multiplication:

$$(f+g)(x)=f(x)+g(x),\qquad (af)(x)=a f(x).$$

A map $u:M'\to M$ induces precomposition $f\mapsto f\circ u$, so Hom is **contravariant** in its first variable. A map $v:N\to N'$ induces postcomposition $f\mapsto v\circ f$, so Hom is **covariant** in its second variable.

The basic natural isomorphism $\operatorname{Hom}_A(A,M)\cong M$ sends $f$ to $f(1)$. Later, bilinear maps yield the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/02 Modules/02.08 Restriction and Extension of Scalars/Tensor-Hom Adjunction\|Tensor-Hom Adjunction]]

$$\operatorname{Hom}_A(M\otimes_A N,P)\cong\operatorname{Hom}_A(M,\operatorname{Hom}_A(N,P)).$$

## Source

- `02_01_modules_and_module_homomorphisms.pdf`, printed p. 18.
