---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/First Isomorphism Theorem for Modules/","title":"First Isomorphism Theorem for Modules","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"],"dg-note-properties":{"title":"First Isomorphism Theorem for Modules","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"]}}
---


# First Isomorphism Theorem for Modules

For every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Foundations/Module Homomorphism\|Module Homomorphism]] $f:M\to N$, there is a natural isomorphism

$$M/\ker f\cong\operatorname{im}f,$$

sending $m+\ker f$ to $f(m)$.

## Why it works

If two elements of $M$ have the same image, their difference lies in $\ker f$, so they determine the same coset. This proves the induced map is well-defined and injective; its codomain is the image, so it is surjective.

## Interpretation

Every linear map decomposes conceptually into

$$M\twoheadrightarrow M/\ker f\xrightarrow{\sim}\operatorname{im}f\hookrightarrow N.$$

It first forgets precisely the relations in the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Kernel of a Module Homomorphism\|kernel]], then identifies the result with the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Image of a Module Homomorphism\|image]], then includes that image into the target.

## Source

- `02_02_submodules_and_quotient_modules.pdf`, printed p. 19.
