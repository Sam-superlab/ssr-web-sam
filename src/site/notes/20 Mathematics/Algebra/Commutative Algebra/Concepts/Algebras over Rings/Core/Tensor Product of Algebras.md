---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Algebras over Rings/Core/Tensor Product of Algebras/","title":"Tensor Product of Algebras","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/algebras-over-rings"],"dg-note-properties":{"title":"Tensor Product of Algebras","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/algebras-over-rings"]}}
---


# Tensor Product of Algebras

For commutative $A$-algebras $B,C$, their **tensor product as algebras** is the module $B\otimes_A C$ with multiplication

$$(b\otimes c)(b'\otimes c')=bb'\otimes cc'$$

and identity $1\otimes1$.

## Universal property

Suppose an $A$-algebra $D$ has $A$-algebra maps $u:B\to D$ and $v:C\to D$. Because the rings are commutative, $(b,c)\mapsto u(b)v(c)$ is $A$-bilinear and induces a unique algebra map

$$B\otimes_A C\longrightarrow D,\qquad b\otimes c\mapsto u(b)v(c).$$

Thus $B\otimes_A C$ is the pushout of $B\leftarrow A\to C$: it combines the two algebras while identifying their images of the base ring.

## Examples

- $A[x]\otimes_A A[y]\cong A[x,y]$.
- $(A/I)\otimes_A(A/J)\cong A/(I+J)$.
- For field extensions, $K\otimes_kL$ need not be a field; it can have zero divisors or nilpotents.

## Source

- `02_11_tensor_product_of_algebras.pdf`, printed pp. 30-31.
