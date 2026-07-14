---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Foundations/Module Homomorphism/","title":"Module Homomorphism","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"],"dg-note-properties":{"title":"Module Homomorphism","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"]}}
---


# Module Homomorphism

For $A$-modules $M$ and $N$, an **$A$-module homomorphism** is a map $f:M\to N$ satisfying

$$f(x+y)=f(x)+f(y),\qquad f(ax)=af(x).$$

It is also called an **$A$-linear map**. Its [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Kernel of a Module Homomorphism\|kernel]] measures failure of injectivity, its [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Image of a Module Homomorphism\|image]] measures what is reached, and its [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Cokernel\|Cokernel]] measures failure of surjectivity.

## Examples

- Multiplication by a fixed $a\in A$, $m\mapsto am$, is $A$-linear.
- The quotient projection $M\to M/N$ is linear when $N$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Submodule\|Submodule]].
- A group homomorphism between $\mathbb Z$-modules is automatically $\mathbb Z$-linear.

## Nonexample

Complex conjugation $\mathbb C\to\mathbb C$ is $\mathbb R$-linear but not $\mathbb C$-linear, illustrating that linearity depends on the chosen scalar ring.

Composition and addition of module homomorphisms are again module homomorphisms. All maps $M\to N$ together form the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Foundations/Hom Module\|Hom Module]].

## Source

- `02_01_modules_and_module_homomorphisms.pdf`, printed p. 18.
