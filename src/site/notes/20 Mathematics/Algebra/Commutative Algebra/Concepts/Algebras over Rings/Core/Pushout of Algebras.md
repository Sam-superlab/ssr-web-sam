---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Algebras over Rings/Core/Pushout of Algebras/","title":"Pushout of Algebras","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/algebras-over-rings"],"dg-note-properties":{"title":"Pushout of Algebras","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/algebras-over-rings"]}}
---


# Pushout of Algebras

Given $A$-algebras $B$ and $C$, a **pushout** is an $A$-algebra $P$ with compatible maps $B\to P$ and $C\to P$ such that every other compatible pair $B\to D$, $C\to D$ factors uniquely through $P$.

In commutative algebra,

$$P=B\otimes_A C.$$

The structure maps are $b\mapsto b\otimes1$ and $c\mapsto1\otimes c$. Compatibility follows from

$$f(a)\otimes1=1\otimes g(a).$$

## Intuition

The pushout combines $B$ and $C$ while forcing their two copies of $A$ to agree, and imposes no extra relations. For example, combining $A[x]$ and $A[y]$ over $A$ produces $A[x,y]$.

The book presents the canonical commutative diagram; the pushout terminology names its universal content.

## Source

- `02_11_tensor_product_of_algebras.pdf`, printed pp. 30-31; canonical algebra diagram following the multiplication construction.
