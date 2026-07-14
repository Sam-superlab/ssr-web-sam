---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Fraction Rings/Field of Fractions/","title":"Field of Fractions","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"],"dg-note-properties":{"title":"Field of Fractions","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/localization-and-fractions"]}}
---


# Field of Fractions

For an integral domain $A$, its **field of fractions** is the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Core/Localization of a Ring\|localization]]

$$
\operatorname{Frac}(A)=(A\setminus\{0\})^{-1}A.
$$

Every element has the form $a/b$ with $b\ne0$, and $A$ embeds by $a\mapsto a/1$.

## Universal property

Any injective homomorphism from $A$ into a field $K$ extends uniquely to a homomorphism $\operatorname{Frac}(A)\to K$ sending $a/b$ to the quotient of the images. Thus the field is canonical up to a unique $A$-isomorphism.

## Examples

- $\operatorname{Frac}(\mathbb Z)=\mathbb Q$.
- $\operatorname{Frac}(k[x])=k(x)$.
- $\operatorname{Frac}(k[x_1,\ldots,x_n])=k(x_1,\ldots,x_n)$.

If $A$ has zero-divisors, $A\setminus\{0\}$ need not be multiplicatively closed: two nonzero zero-divisors can have product $0$. The appropriate replacement is the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Fraction Rings/Total Ring of Fractions\|Total Ring of Fractions]], which inverts only non-zero-divisors.

## Source

- 03_00_rings_and_modules_of_fractions.pdf, introductory discussion and A&M Remark after Proposition 3.1, printed pp. 36--37.
