---
{"dg-publish":true,"permalink":"/Mainfolder/Mathematics/General vector space/"}
---


# Beyond Two Dimensions

## Section 4.1: Vector Spaces and Subspaces

>[!theorem] Proposition 4.1.7
>Let $V$ be a vector space.
>1. For all $\vec{v} \in V$, we have $\vec{0} + \vec{v} = \vec{v}$
>2. For all $\vec{v}, \vec{w} \in V$, if $\vec{v} + \vec{w} = \vec{0}$, then $\vec{w} + \vec{v} = \vec{0}$

>[!theorem] Proposition 4.1.8
>Suppose that $V$ is a vector space, and let $\vec{u}, \vec{v}, \vec{w} \in V$.
>1. If $\vec{v} + \vec{u} = \vec{w} + \vec{u}$, then $\vec{v} = \vec{w}$
>2. If $\vec{u} + \vec{v} = \vec{u} + \vec{w}$, then $\vec{v} = \vec{w}$

>[!theorem] Proposition 4.1.9
>Let $V$ be a vector space.
>1. If $\vec{z} \in V$ and $\vec{v} + \vec{z} = \vec{v}$ for all $\vec{v} \in V$, then $\vec{z} = \vec{0}$, i.e. $\vec{0}$ is the only additive identity
>2. For all $\vec{v} \in V$, there is a unique $\vec{w} \in V$ with $\vec{v} + \vec{w} = \vec{0}$, i.e. additive inverses are unique

>[!theorem] Proposition 4.1.11
>Let $V$ be a vector space.
>1. $0 \cdot \vec{v} = \vec{0}$ for all $\vec{v} \in V$
>2. $c \cdot \vec{0} = \vec{0}$ for all $c \in \mathbb{R}$
>3. $(-1) \cdot \vec{v} = -\vec{v}$ for all $\vec{v} \in V$

>[!theorem] Proposition 4.1.16
>Let $V$ be a vector space and let $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in V$. The set $Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ is a subspace of $V$

## Section 4.2: Solving Linear Systems

>[!theorem] Proposition 4.2.4 (Elementary Row Operations are Reversible)
>Suppose that we have a linear system, and we apply one elementary row operation to obtain a new system. We can then apply one elementary row operation to the new system in order to recover the old system.

>[!theorem] Corollary 4.2.5
>Suppose that we have a linear system $A_1$, and we apply one elementary row operation to obtain a new system $A_2$. If $S_1$ is the solution set to the original system, and $S_2$ is the solution set to the new system, then $S_1 = S_2$.

>[!theorem] Proposition 4.2.11
>For any matrix $A$, there exists an echelon form of $A$.

>[!theorem] Proposition 4.2.12
>Suppose that we have a linear system with augmented matrix $A$, and that $B$ is an echelon form of $A$.
>1. If the last column of $B$ contains a leading entry, then the system is inconsistent
>2. If the last column of $B$ contains no leading entry, but every other column of $B$ has a leading entry, then the system is consistent and has a unique solution
>3. If the last column of $B$ contains no leading entry, and there is at least one other column of $B$ without a leading entry, then the system is consistent and has infinitely many solutions. Moreover, for each choice of values for the variables that do not correspond to leading entries, there is a unique solution for the system taking these values.

>[!theorem] Proposition 4.2.15
>Let $a_0, a_1, \dots, a_n \in \mathbb{R}$ and $b_0, b_1, \dots, b_n \in \mathbb{R}$. Let $f : \mathbb{R} \to \mathbb{R}$ and $g : \mathbb{R} \to \mathbb{R}$ be the polynomial functions: $f(x) = a_nx^n + a_{n-1}x^{n-1} + \dots + a_1x + a_0$ and $g(x) = b_nx^n + b_{n-1}x^{n-1} + \dots + b_1x + b_0$. If $f(x) = g(x)$ for all $x \in \mathbb{R}$, then $a_i = b_i$ for all $i$.

## Section 4.3: Spanning Sequences

>[!theorem] Proposition 4.3.1
>Let $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in \mathbb{R}^m$. Let $A$ be the $m \times n$ matrix where the $i^{th}$ column is $\vec{u}_i$, and let $B$ be an echelon form of $A$. We then have that $Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n) = \mathbb{R}^m$ if and only if every row of $B$ has a leading entry.

>[!theorem] Corollary 4.3.2
>If $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in \mathbb{R}^m$ and $Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n) = \mathbb{R}^m$, then $n \ge m$.

>[!theorem] Corollary 4.3.3
>If $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in \mathbb{R}^m$ and $n < m$, then $Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n) \ne \mathbb{R}^m$.

## Section 4.4: Linear Independence

>[!theorem] Proposition 4.4.2
>Let $V$ be a vector space, and let $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in V$ where $n \ge 2$. The following are equivalent:
>1. $(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ is linearly independent
>2. There does not exist an $i$ such that $\vec{u}_i \in Span(\vec{u}_1, \dots, \vec{u}_{i-1}, \vec{u}_{i+1}, \dots, \vec{u}_n)$

>[!theorem] Proposition 4.4.3
>Let $V$ be a vector space, and let $\vec{u} \in V$. We then have that $(\vec{u})$ is linearly independent if and only if $\vec{u} \ne \vec{0}$.

>[!theorem] Proposition 4.4.5
>Let $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in \mathbb{R}^m$. Let $A$ be the $m \times n$ matrix where the $i^{th}$ column is $\vec{u}_i$, and let $B$ be an echelon form of $A$. We then have that $(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ is linearly independent if and only if every column of $B$ has a leading entry.

>[!theorem] Corollary 4.4.6
>If $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in \mathbb{R}^m$ and $(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ is linearly independent, then $n \le m$.

>[!theorem] Corollary 4.4.7
>If $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in \mathbb{R}^m$ and $n > m$, then $(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ is linearly dependent.

## Section 4.5: Bases and Coordinates

>[!theorem] Theorem 4.5.2
>Let $V$ be a vector space and let $\alpha = (\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ be a sequence of elements of $V$. We then have that $\alpha$ is a basis for $V$ if and only if every $\vec{v} \in V$ can be expressed as a linear combination of $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n$ in a unique way.

>[!theorem] Proposition 4.5.4
>Let $V$ be a vector space and let $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n, \vec{w} \in V$. The following are equivalent:
>1. $Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n, \vec{w}) = Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$
>2. $\vec{w} \in Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$

>[!theorem] Proposition 4.5.5
>Let $V$ be a vector space, and let $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in V$ be such that $Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n) = V$. There exists a basis of $V$ that can be obtained by omitting some of the $\vec{u}_i$ from the sequence.

>[!theorem] Proposition 4.5.6
>Let $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in \mathbb{R}^m$, and let $W = Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$. Let $A$ be the $m \times n$ matrix whose $i^{th}$ column is $\vec{u}_i$, and let $B$ be an echelon form of $A$. If we build the sequence consisting only of those $\vec{u}_i$ such that the $i^{th}$ column of $B$ has a leading entry, then we obtain a basis for $W$.

## Section 4.6: Dimension

>[!theorem] Proposition 4.6.1 (Steinitz Exchange)
>Let $V$ be a vector space and let $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n, \vec{w} \in V$. Suppose that we have $d_1, \dots, d_n \in \mathbb{R}$ with $\vec{w} = d_1\vec{u}_1 + \dots + d_k\vec{u}_k + \dots + d_n\vec{u}_n$. If $d_k \ne 0$, then $Span(\vec{u}_1, \dots, \vec{u}_k, \dots, \vec{u}_n) = Span(\vec{u}_1, \dots, \vec{u}_{k-1}, \vec{w}, \vec{u}_{k+1}, \dots, \vec{u}_n)$.

>[!theorem] Theorem 4.6.2
>Let $V$ be a vector space and let $\vec{u}_1, \dots, \vec{u}_n, \vec{w}_1, \dots, \vec{w}_m \in V$. If $m > n$ and $Span(\vec{u}_1, \dots, \vec{u}_n) = V$, then $(\vec{w}_1, \dots, \vec{w}_m)$ is linearly dependent.

>[!theorem] Corollary 4.6.3
>Let $V$ be a vector space and let $\vec{u}_1, \dots, \vec{u}_n, \vec{w}_1, \dots, \vec{w}_m \in V$ be such that both $Span(\vec{u}_1, \dots, \vec{u}_n) = V$ and $(\vec{w}_1, \dots, \vec{w}_m)$ is linearly independent. We then have $m \le n$.

>[!theorem] Corollary 4.6.4
>Suppose that $V$ is a vector space and both $(\vec{u}_1, \dots, \vec{u}_n)$ and $(\vec{w}_1, \dots, \vec{w}_m)$ are bases for $V$. We then have that $m = n$.

>[!theorem] Proposition 4.6.7
>Let $V$ be a finite-dimensional vector space and let $n = dim(V)$. Let $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in V$.
>1. If $(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ is linearly independent, then $(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ is a basis of $V$
>2. If $Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n) = V$, then $(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ is a basis of $V$

>[!theorem] Proposition 4.6.8
>Let $V$ be a finite-dimensional vector space with $dim(V) = n$, and let $W$ be a subspace of $V$. There exists $k \in \{0, 1, \dots, n\}$ and $\vec{w}_1, \dots, \vec{w}_k \in W$ with $W = Span(\vec{w}_1, \dots, \vec{w}_k)$ and such that $(\vec{w}_1, \dots, \vec{w}_k)$ is linearly independent. In particular, $W$ is a finite-dimensional vector space and $dim(W) \le dim(V)$.

>[!theorem] Proposition 4.6.9
>Let $V$ be a vector space, let $(\vec{u}_1, \dots, \vec{u}_n)$ be a linearly independent sequence of vectors in $V$, and let $\vec{w} \in V$. The following are equivalent:
>1. $(\vec{u}_1, \dots, \vec{u}_n, \vec{w})$ is linearly independent
>2. $\vec{w} \notin Span(\vec{u}_1, \dots, \vec{u}_n)$

>[!theorem] Proposition 4.6.10
>Let $V$ be a finite-dimensional vector space, and let $(\vec{u}_1, \dots, \vec{u}_k)$ be a linearly independent sequence of vectors in $V$. There exists $\vec{w}_1, \dots, \vec{w}_m \in V$ (possibly with $m = 0$) such that $(\vec{u}_1, \dots, \vec{u}_k, \vec{w}_1, \dots, \vec{w}_m)$ is a basis of $V$.
