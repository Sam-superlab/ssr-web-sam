---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/01 Rings and Ring Homomorphisms/","dg-note-properties":{}}
---


# Rings and Ring Homomorphisms

A [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring\|Ring]] $A$ has addition and multiplication. Addition makes $A$ an abelian group; multiplication is associative and distributes over addition. Atiyah and Macdonald impose two standing conventions:

- multiplication is commutative;
- there is a multiplicative identity $1$.

The convention permits $1=0$. In that case every $x\in A$ satisfies $x=x1=x0=0$, so $A$ is the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Zero Ring\|Zero Ring]].

A [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring Homomorphism\|Ring Homomorphism]] $f:A\to B$ preserves addition, multiplication, and identity:

$$
f(x+y)=f(x)+f(y),\qquad f(xy)=f(x)f(y),\qquad f(1_A)=1_B.
$$

Consequently it preserves $0$, negatives, subtraction, and every integer combination. Homomorphisms compose, and the identity map is a homomorphism.

A [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Subring\|Subring]] $S\subseteq A$ uses the operations inherited from $A$ and must contain the same identity. The inclusion $S\hookrightarrow A$ is then a ring homomorphism. A bijective homomorphism is a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring Isomorphism\|Ring Isomorphism]]: it says that two rings have the same algebraic structure under different names.

## Examples

- $\mathbb Z$, $\mathbb Q$, and $k[x_1,\ldots,x_n]$ are rings.
- Evaluation at $a\in k$ defines $k[x]\to k$, $f(x)\mapsto f(a)$.
- The inclusion $\mathbb Z\hookrightarrow\mathbb Q$ is a homomorphism but not an isomorphism.
- The set $2\mathbb Z\subseteq\mathbb Z$ is closed under addition and multiplication, but it is not a subring under the book's convention because it does not contain $1$.

## Why maps matter

The next section associates to every homomorphism its [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Kernel of a Ring Homomorphism\|kernel]] and [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Image of a Ring Homomorphism\|image]]. The kernel is the ideal of relations killed by the map, and the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/First Isomorphism Theorem for Rings\|First Isomorphism Theorem for Rings]] reconstructs the image as a quotient by those relations.

## Source

- 01_01_rings_and_ring_homomorphisms.pdf, printed p. 1; the homomorphism and subring definitions continue at the start of 01_02_ideals_quotient_rings.pdf, printed p. 2.
