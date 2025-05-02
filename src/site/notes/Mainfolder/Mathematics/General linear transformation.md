---
{"dg-publish":true,"permalink":"/Mainfolder/Mathematics/General linear transformation/"}
---


# Linear Transformations and Matrices

## Section 5.1: Linear Transformations

>[!theorem] Proposition 5.1.2
>Let $m, n \in \mathbb{N}^+$ and suppose that we have numbers $a_{i,j} \in \mathbb{R}$ for all $i, j \in \mathbb{N}$ with both $1 \le i \le m$ and $1 \le j \le n$. Define $T : \mathbb{R}^n \to \mathbb{R}^m$ by
>$$T\left(\begin{pmatrix} x_1 \\ x_2 \\ \vdots \\ x_n \end{pmatrix}\right) = \begin{pmatrix} a_{1,1}x_1 + a_{1,2}x_2 + \dots + a_{1,n}x_n \\ a_{2,1}x_1 + a_{2,2}x_2 + \dots + a_{2,n}x_n \\ \vdots \\ a_{m,1}x_1 + a_{m,2}x_2 + \dots + a_{m,n}x_n \end{pmatrix}$$
>We then have that T is a linear transformation.

>[!theorem] Proposition 5.1.3
>Let $V$ be a vector space and let $\alpha$ be a basis of $V$ with $n$ elements. The function $Coord_\alpha : V \to \mathbb{R}^n$ is a linear transformation.

>[!theorem] Proposition 5.1.4
>Let $T : V \to W$ be a linear transformation. We have the following:
>1. $T(\vec{0}_V) = \vec{0}_W$ (where $\vec{0}_V$ is the zero vector of $V$, and $\vec{0}_W$ is the zero vector of $W$)
>2. $T(-\vec{v}) = -T(\vec{v})$ for all $\vec{v} \in V$
>3. $T(c_1\vec{v}_1 + c_2\vec{v}_2) = c_1 \cdot T(\vec{v}_1) + c_2 \cdot T(\vec{v}_2)$ for all $\vec{v}_1, \vec{v}_2 \in V$ and all $c_1, c_2 \in \mathbb{R}$

>[!theorem] Theorem 5.1.5
>Let $V$ and $W$ be vector spaces, and suppose that $Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n) = V$. Suppose that $T : V \to W$ and $S : V \to W$ are linear transformations with the property that $T(\vec{u}_i) = S(\vec{u}_i)$ for all $i \in \{1, 2, \dots, n\}$. We then have that $T = S$, i.e. $T(\vec{v}) = S(\vec{v})$ for all $\vec{v} \in V$.

>[!theorem] Theorem 5.1.6
>Let $V$ and $W$ be vector spaces, and suppose that $(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ is a basis of $V$. Let $\vec{w}_1, \vec{w}_2, \dots, \vec{w}_n \in W$. There exists a unique linear transformation $T : V \to W$ with $T(\vec{u}_i) = \vec{w}_i$ for all $i \in \{1, 2, \dots, n\}$.

>[!theorem] Proposition 5.1.9
>Let $T : V \to W$ be a linear transformation, let $\alpha = (\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ be a basis for $V$, and let $\beta = (\vec{w}_1, \vec{w}_2, \dots, \vec{w}_m)$ be a basis for $W$. Suppose that $[T]^\beta_\alpha = \begin{pmatrix} a_{1,1} & a_{1,2} & \dots & a_{1,n} \\ a_{2,1} & a_{2,2} & \dots & a_{2,n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m,1} & a_{m,2} & \dots & a_{m,n} \end{pmatrix}$ and that $[\vec{v}]_\alpha = \begin{pmatrix} c_1 \\ c_2 \\ \vdots \\ c_n \end{pmatrix}$. We then have that $[T(\vec{v})]_\beta = c_1 \cdot [T(\vec{u}_1)]_\beta + c_2 \cdot [T(\vec{u}_2)]_\beta + \dots + c_n \cdot [T(\vec{u}_n)]_\beta$, and hence $[T(\vec{v})]_\beta = \begin{pmatrix} a_{1,1}c_1 + a_{1,2}c_2 + \dots + a_{1,n}c_n \\ a_{2,1}c_1 + a_{2,2}c_2 + \dots + a_{2,n}c_n \\ \vdots \\ a_{m,1}c_1 + a_{m,2}c_2 + \dots + a_{m,n}c_n \end{pmatrix}$.

>[!theorem] Proposition 5.1.12
>Let $V$ and $W$ be vector spaces, and let $T, S : V \to W$ be linear transformations.
>1. The function $T + S$ is a linear transformation
>2. For all $r \in \mathbb{R}$, then function $r \cdot T$ is a linear transformation

>[!theorem] Proposition 5.1.15
>Let $V$ and $W$ be vector spaces, let $T : V \to W$ and $S : V \to W$ be linear transformations, let $\alpha = (\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ be a basis for $V$, and let $\beta = (\vec{w}_1, \vec{w}_2, \dots, \vec{w}_m)$ be a basis for $W$. We have the following:
>1. $[T + S]^\beta_\alpha = [T]^\beta_\alpha + [S]^\beta_\alpha$
>2. $[c \cdot T]^\beta_\alpha = c \cdot [T]^\beta_\alpha$ for all $c \in \mathbb{R}$

>[!theorem] Proposition 5.1.16
>Let $V, Z,$ and $W$ be vector spaces, and let $T : Z \to W$ and $S : V \to Z$ be linear transformations. We then have that $T \circ S : V \to W$ is a linear transformation.

>[!theorem] Proposition 5.1.18
>Let $V, Z,$ and $W$ be finite-dimensional vector spaces, and let $T : Z \to W$ and $S : V \to Z$ be linear transformations. Let $\alpha$ be a basis for $V$, let $\gamma$ be a basis for $Z$, and let $\beta$ be a basis for $W$. We then have $[T \circ S]^\beta_\alpha = [T]^\beta_\gamma \cdot [S]^\gamma_\alpha$.

## Section 5.2: The Range and Null Space of a Linear Transformation

>[!theorem] Proposition 5.2.2
>Let $V$ and $W$ be vector spaces, and let $T : V \to W$ be a linear transformation.
>1. $Null(T)$ is a subspace of $V$
>2. $range(T)$ is a subspace of $W$

>[!theorem] Proposition 5.2.3
>Let $T : \mathbb{R}^n \to \mathbb{R}^m$ be a linear transformation, and let $\vec{b} \in \mathbb{R}^m$. The following are equivalent:
>1. $\vec{b} \in range(T)$
>2. $\vec{b}$ is a linear combination of the columns of $[T]$
>Thus, $range(T)$ is the span of the columns of $[T]$

>[!theorem] Corollary 5.2.4
>Let $T : \mathbb{R}^n \to \mathbb{R}^m$ be a linear transformation, and let $B$ be an echelon form of the matrix $[T]$. The following are equivalent:
>1. $T$ is surjective
>2. Every row of $B$ has a leading entry

>[!theorem] Corollary 5.2.5
>Let $T : \mathbb{R}^n \to \mathbb{R}^m$ be a linear transformation and let $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in \mathbb{R}^m$ be the columns of $[T]$. Let $B$ be an echelon form of the matrix $[T]$. If we build the sequence consisting only of those $\vec{u}_i$ such that the $i^{th}$ column of $B$ has a leading entry, then we obtain a basis for $range(T)$.

>[!theorem] Proposition 5.2.6
>Let $V$ and $W$ be vector spaces, and let $T : V \to W$ be a linear transformation.
>1. If $T(\vec{v}) = \vec{b}$ and $\vec{z} \in Null(T)$, then $T(\vec{v} + \vec{z}) = \vec{b}$
>2. If $T(\vec{v}_1) = \vec{b}$ and $T(\vec{v}_2) = \vec{b}$, then $\vec{v}_1 - \vec{v}_2 \in Null(T)$

>[!theorem] Corollary 5.2.7
>Let $T : V \to W$ be a linear transformation, and let $\vec{b} \in W$. Suppose that $\vec{v} \in V$ is such that $T(\vec{v}) = \vec{b}$. We have $\{\vec{x} \in V : T(\vec{x}) = \vec{b}\} = \{\vec{v} + \vec{z} : \vec{z} \in Null(T)\}$.

>[!theorem] Corollary 5.2.9
>Let $T : \mathbb{R}^n \to \mathbb{R}^m$ be a linear transformation, and let $B$ be an echelon form of $[T]$. We then have that $rank(T)$ is the number of leading entries in $B$.

>[!theorem] Theorem 5.2.10 (Rank-Nullity Theorem)
>Let $T : V \to W$ be a linear transformation with $V$ and $W$ finite-dimensional vector spaces. We then have that $rank(T) + nullity(T) = dim(V)$.

>[!theorem] Proposition 5.2.11
>Let $T : V \to W$ be a linear transformation. We have that $T$ is injective if and only if $Null(T) = \{\vec{0}_V\}$.

>[!theorem] Proposition 5.2.12
>Let $V$ and $W$ be vector spaces. Let $T : V \to W$ be an injective linear transformation and let $(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ be a linearly independent sequence in $V$. We then have that $(T(\vec{u}_1), T(\vec{u}_2), \dots, T(\vec{u}_n))$ is a linearly independent sequence in $W$.

>[!theorem] Proposition 5.2.13
>Let $V$ and $W$ be vector spaces. Let $T : V \to W$ be a surjective linear transformation and assume that $Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n) = V$. We then have that $Span(T(\vec{u}_1), T(\vec{u}_2), \dots, T(\vec{u}_n)) = W$.

>[!theorem] Corollary 5.2.14
>Let $V$ and $W$ be finite-dimensional vector spaces, and let $n = dim(V)$ and $m = dim(W)$. Let $T : V \to W$ be a linear transformation.
>1. If $T$ is injective, then $n \le m$
>2. If $T$ is surjective, then $m \le n$
>3. If $T$ is bijective, then $m = n$

>[!theorem] Proposition 5.2.15
>Suppose that $T : V \to W$ is a bijective linear transformation. We then have that the function $T^{-1} : W \to V$ is a linear transformation.

>[!theorem] Proposition 5.2.17
>Let $A$ be an $n \times n$ matrix, and let $B$ be an echelon form of $A$. We then have that $A$ is invertible if and only if every row and every column of $B$ has a leading entry.

## Section 5.3: Determinants

>[!theorem] Theorem 5.3.2
>For each $n \in \mathbb{N}^+$, there is a unique function $f$ satisfying the determinant properties. We call this function det.

>[!theorem] Proposition 5.3.3
>Let $\vec{v}_1, \vec{v}_2, \dots, \vec{v}_n \in \mathbb{R}^n$. If $i < j$, then $det(\vec{v}_1, \dots, \vec{v}_i, \dots, \vec{v}_j, \dots, \vec{v}_n) = - det(\vec{v}_1, \dots, \vec{v}_j, \dots, \vec{v}_i, \dots, \vec{v}_n)$.

>[!theorem] Proposition 5.3.4
>Let $\vec{v}_1, \vec{v}_2, \dots, \vec{v}_n \in \mathbb{R}^n$ and let $c \in \mathbb{R}$. If $i < j$ and $c \in \mathbb{R}$, then $det(\vec{v}_1, \dots, \vec{v}_i, \dots, \vec{v}_j + c\vec{v}_i, \dots, \vec{v}_n) = det(\vec{v}_1, \dots, \vec{v}_i, \dots, \vec{v}_j, \dots, \vec{v}_n)$ and $det(\vec{v}_1, \dots, \vec{v}_i + c\vec{v}_j, \dots, \vec{v}_j, \dots, \vec{v}_n) = det(\vec{v}_1, \dots, \vec{v}_i, \dots, \vec{v}_j, \dots, \vec{v}_n)$.

>[!theorem] Proposition 5.3.5
>Let $\vec{v}_1, \vec{v}_2, \dots, \vec{v}_n \in \mathbb{R}^n$ and assume that $(\vec{v}_1, \vec{v}_2, \dots, \vec{v}_n)$ is linearly dependent. We then have that $det(\vec{v}_1, \vec{v}_2, \dots, \vec{v}_n) = 0$.

>[!theorem] Proposition 5.3.8
>Suppose that $A$ and $B$ are $n \times n$ matrices with $A \sim_R B$. We then have that $det(A) = 0$ if and only if $det(B) = 0$.

>[!theorem] Proposition 5.3.9
>If $A$ is an $n \times n$ diagonal matrix with $A = \begin{pmatrix} a_{1,1} & 0 & \dots & 0 \\ 0 & a_{2,2} & \dots & 0 \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & \dots & a_{n,n} \end{pmatrix}$, then $det(A) = a_{1,1}a_{2,2} \dots a_{n,n}$.

>[!theorem] Proposition 5.3.10
>If $A$ is an $n \times n$ upper triangular matrix, i.e. if $A = \begin{pmatrix} a_{1,1} & a_{1,2} & \dots & a_{1,n} \\ 0 & a_{2,2} & \dots & a_{2,n} \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & \dots & a_{n,n} \end{pmatrix}$, then $det(A) = a_{1,1}a_{2,2} \dots a_{n,n}$.

>[!theorem] Corollary 5.3.11
>If $A$ is a square matrix, then $A$ is invertible if and only if $det(A) \ne 0$.

>[!theorem] Theorem 5.3.12
>For any $n \times n$ matrix $A$, we have $det(A) = det(A^T)$.

>[!theorem] Theorem 5.3.14
>Let $A$ be an $n \times n$ matrix. For any $i$, we have $det(A) = a_{i1}C_{i1} + a_{i2}C_{i2} + \dots + a_{in}C_{in}$ and for any $j$, we have $det(A) = a_{1j}C_{1j} + a_{2j}C_{2j} + \dots + a_{nj}C_{nj}$.

>[!theorem] Theorem 5.3.15
>If $A$ and $B$ are $n \times n$ matrices, then $det(AB) = det(A) \cdot det(B)$.

## Section 5.4: Eigenvalues and Eigenvectors

>[!theorem] Proposition 5.4.2
>Let $T : V \to V$ be a linear transformation and let $\lambda \in \mathbb{R}$. The set $W = \{\vec{v} \in V : T(\vec{v}) = \lambda\vec{v}\}$, which is the set of all eigenvectors of $T$ corresponding to $\lambda$ together with $\vec{0}$, is a subspace of $V$.

>[!theorem] Proposition 5.4.4
>Let $A$ be an $n \times n$ matrix, let $\vec{v} \in \mathbb{R}^n$, and let $\lambda \in \mathbb{R}$. We have that $A\vec{v} = \lambda\vec{v}$ if and only if $\vec{v} \in Null(A - \lambda I)$. Therefore, $\vec{v}$ is an eigenvector of $A$ corresponding to $\lambda$ if and only if $\vec{v} \ne \vec{0}$ and $\vec{v} \in Null(A - \lambda I)$.

>[!theorem] Corollary 5.4.5
>Let $A$ be an $n \times n$ matrix and let $\lambda \in \mathbb{R}$. We have that $\lambda$ is an eigenvalue of $A$ if and only if $Null(A - \lambda I) \ne \{\vec{0}\}$.

>[!theorem] Proposition 5.4.7
>If $A$ is an $n \times n$ matrix, then the characteristic polynomial of $A$ is a polynomial of degree $n$.

>[!theorem] Proposition 5.4.10
>Let $V$ be a finite-dimensional vector space, let $T : V \to V$ be a linear transformation and let $\alpha = (\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ be a basis of $V$. The following are equivalent:
>1. $[T]^\alpha_\alpha$ is a diagonal matrix
>2. $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n$ are all eigenvectors of $T$
>Furthermore, in this case, the diagonal entries of $[T]^\alpha_\alpha$ are the eigenvalues corresponding to $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n$.

>[!theorem] Corollary 5.4.11
>Let $V$ be a finite-dimensional vector space and let $T : V \to V$ be a linear transformation. We then have that $T$ is diagonalizable if and only if there exists a basis of $V$ consisting entirely of eigenvectors of $T$.



