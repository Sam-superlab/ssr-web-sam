---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Tensor Product of Module Homomorphisms/","title":"Tensor Product of Module Homomorphisms","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"],"dg-note-properties":{"title":"Tensor Product of Module Homomorphisms","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/homological-algebra"]}}
---


# Tensor Product of Module Homomorphisms

Given $A$-linear maps $f:M\to M'$ and $g:N\to N'$, their **tensor product** is the unique map

$$f\otimes g:M\otimes_A N\to M'\otimes_A N'$$

satisfying

$$(f\otimes g)(x\otimes y)=f(x)\otimes g(y).$$

Existence follows because $(x,y)\mapsto f(x)\otimes g(y)$ is [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Tensor Products/Bilinear Map\|bilinear]].

Tensor products respect identities and composition:

$$(f'\circ f)\otimes(g'\circ g)=(f'\otimes g')\circ(f\otimes g).$$

This functoriality lets one tensor an entire [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Exact Sequences/Exact Sequence\|Exact Sequence]] with a fixed module. The resulting sequence is always right exact, but its left edge can fail unless the fixed module is [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Homological Algebra/Flatness and Tor/Flat Module\|flat]].

## Source

- `02_07_tensor_product_of_modules.pdf`, printed p. 27, after Exercise 2.15.
