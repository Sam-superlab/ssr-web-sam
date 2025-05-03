---
{"dg-publish":true,"permalink":"/Mainfolder/Mathematics/General linear transformation/"}
---


# Linear Transformations and Matrices

## Section 5.1: Linear Transformations

**Core Idea: Generalizing Structure-Preserving Maps**

Having established the general notion of a Vector Space in Chapter 4, Section 5.1 aims to define the most important type of function *between* vector spaces: those that respect the underlying vector space operations (addition and scalar multiplication). These are called **Linear Transformations**.

**Rationale for the Definition (Definition 5.1.1):**

1.  **What properties should a "natural" or "structure-preserving" map $T: V \to W$ have?** Since vector spaces are defined by their addition and scalar multiplication, a natural map should interact nicely with these.
2.  **Preserving Addition:** If we add two vectors in $V$ and then apply $T$, we should get the same result as if we first apply $T$ to each vector individually and then add the results in $W$. That is, $T(\vec{v}_1 + \vec{v}_2) = T(\vec{v}_1) + T(\vec{v}_2)$.
3.  **Preserving Scalar Multiplication:** If we scale a vector in $V$ by $c$ and then apply $T$, we should get the same result as if we first apply $T$ to the vector and then scale the result in $W$ by $c$. That is, $T(c \cdot \vec{v}) = c \cdot T(\vec{v})$.
4.  **The Definition:** These two essential properties become the *definition* of a linear transformation. It's a function between vector spaces that "plays nice" with the operations that define those spaces.
5.  **Broad Applicability:** This definition is abstract enough to apply not just to functions between $\mathbb{R}^n$ and $\mathbb{R}^m$, but also to functions involving spaces of functions, matrices, etc., as seen in the examples (differentiation, integration). This abstraction allows for unifying concepts across different mathematical domains.

**Rationale for Key Theorems (Uniqueness, Existence, Representation):**

1.  **Linearity Means Determined by Basis Action (Theorem 5.1.5):** If we know what a linear transformation $T$ does to a set of vectors that *span* the domain $V$ (in particular, a basis), then we know what it does to *every* vector in $V$.
    * **Rationale:** Any $\vec{v} \in V$ can be written as a linear combination of the spanning vectors, say $\vec{v} = c_1\vec{u}_1 + \dots + c_n\vec{u}_n$. Because $T$ preserves addition and scalar multiplication, we have $T(\vec{v}) = c_1T(\vec{u}_1) + \dots + c_nT(\vec{u}_n)$. So, the value of $T(\vec{v})$ is completely determined by the values $T(\vec{u}_i)$. This means linear transformations are highly structured; their behavior isn't arbitrary but fixed by their action on a relatively small set.
2.  **Freedom to Define on a Basis (Theorem 5.1.6):** We can define a linear transformation $T: V \to W$ simply by choosing where each basis vector of $V$ should map to in $W$. For any choice of target vectors $\vec{w}_1, \dots, \vec{w}_n \in W$, there exists a *unique* linear transformation $T$ such that $T(\vec{u}_i) = \vec{w}_i$ for a basis $(\vec{u}_1, \dots, \vec{u}_n)$ of $V$.
    * **Rationale:** This theorem guarantees existence and flexibility. It tells us that bases provide complete freedom to construct linear transformations with desired properties. We don't need a "formula" for $T$; specifying its action on a basis is enough to uniquely determine a valid linear $T$.
3.  **Matrix Representation $[T]_\alpha^\beta$ (Definition 5.1.7):** Since $T$ is determined by $T(\vec{u}_1), \dots, T(\vec{u}_n)$ (where $\alpha=(\vec{u}_i)$ is a basis for $V$), and each $T(\vec{u}_i)$ can be uniquely represented by its coordinates relative to a basis $\beta$ of $W$, we can encode the *entire* transformation $T$ as a matrix whose columns are these coordinate vectors $[T(\vec{u}_i)]_\beta$.
    * **Rationale:** This provides a concrete way to represent potentially abstract linear transformations using a grid of numbers (a matrix). It bridges the abstract theory of linear transformations with the computational tools of matrix algebra. The choice of bases $\alpha$ and $\beta$ acts like choosing coordinate systems or "languages" to describe the transformation.
4.  **Matrix Operations Mirror Transformation Operations (Prop 5.1.15, 5.1.18):** The definitions for adding matrices, multiplying a matrix by a scalar, and multiplying matrices are specifically chosen so that they correspond precisely to adding linear transformations, scaling linear transformations, and composing linear transformations, respectively, when viewed through their matrix representations relative to fixed bases.
    * **Rationale:** This ensures that matrix algebra is a faithful computational model for the algebra of linear transformations. We can perform manipulations on matrices (which are often easier to compute with) and know that the results accurately reflect operations on the underlying functions. The complex-looking definition of matrix multiplication, for example, is exactly what's needed to make $[T \circ S] = [T] \cdot [S]$ work out.

In summary, Section 5.1 generalizes the idea of "structure-preserving maps" between vector spaces. The rationale is to define transformations based on the core vector space operations (addition and scalar multiplication), allowing the theory to apply broadly. Key results establish that these transformations are determined by their action on a basis and can be represented concretely by matrices once bases are chosen, with matrix operations directly mirroring the operations on the transformations themselves.

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

**Core Idea: Understanding the Input-Output Behavior of Linear Transformations**

Given a linear transformation $T: V \to W$, this section introduces two fundamental subspaces that help us understand what $T$ "does" to the vectors in $V$:

1.  **Range (Where do the outputs land?):** What vectors in the codomain $W$ are actually "hit" by the transformation $T$?
2.  **Null Space (What inputs get "lost"?):** Which vectors in the domain $V$ get mapped to the zero vector $\vec{0}_W$ in the codomain?

**Rationale for Range(T):**

* **Definition:** $range(T) = \{ \vec{w} \in W \,:\, \exists \vec{v} \in V \text{ with } T(\vec{v}) = \vec{w} \}$. It's simply the set of all achievable outputs.
* **Why Study It?** The range tells us the "reach" of the transformation. Knowing the range is equivalent to knowing which equations of the form $T(\vec{v}) = \vec{w}$ have solutions. It directly relates to whether $T$ is **surjective** (onto) – $T$ is surjective if and only if $range(T) = W$.
* **Subspace Property (Prop 5.2.2):** The range isn't just any subset of $W$; it's a subspace.
    * **Rationale:** This means the set of outputs inherits the algebraic structure of $W$. Linear combinations of achievable outputs are themselves achievable outputs, because $T$ is linear. This structure makes the range easier to analyze (e.g., finding a basis for it).
* **Connection to Columns (Prop 5.2.3):** For $T: \mathbb{R}^n \to \mathbb{R}^m$ with standard matrix $A = [\vec{a}_1 | \dots | \vec{a}_n]$, the range is the span of the columns of $A$: $range(T) = Col(A) = Span(\vec{a}_1, \dots, \vec{a}_n)$.
    * **Rationale:** Any output $T(\vec{x}) = A\vec{x}$ is, by definition of matrix-vector multiplication, equal to $x_1\vec{a}_1 + \dots + x_n\vec{a}_n$. Thus, the set of all outputs ($range(T)$) is precisely the set of all linear combinations of the columns ($Col(A)$). This gives a very concrete way to compute and understand the range for standard matrix transformations.

**Rationale for Null Space (Kernel) Null(T) (Definition 5.2.1):**

* **Definition:** $Null(T) = \{ \vec{v} \in V \,:\, T(\vec{v}) = \vec{0}_W \}$. It's the set of all inputs mapped to the zero vector.
* **Why Study It?** The null space captures what the transformation "collapses" or "nullifies". If $Null(T)$ contains only $\vec{0}_V$, then $T$ distinguishes every non-zero vector from $\vec{0}_V$. If $Null(T)$ contains non-zero vectors, it means multiple distinct input vectors are being mapped to the same output vector $\vec{0}_W$. As we'll see, this relates directly to whether $T$ is **injective** (one-to-one).
* **Subspace Property (Prop 5.2.2):** The null space is a subspace of the *domain* $V$.
    * **Rationale:** This confirms that the set of inputs mapping to zero has a stable algebraic structure. If $\vec{v}_1$ and $\vec{v}_2$ map to $\vec{0}_W$, so does $\vec{v}_1 + \vec{v}_2$ and $c\vec{v}_1$, because $T$ is linear.
* **Connection to Homogeneous Systems:** For $T: \mathbb{R}^n \to \mathbb{R}^m$ with standard matrix $A$, $Null(T)$ is exactly the solution set of the homogeneous system $A\vec{x} = \vec{0}$. This provides a direct computational method (Gaussian elimination) for finding the null space.

**Rationale for Rank, Nullity, and the Rank-Nullity Theorem:**

* **Rank and Nullity (Def 5.2.8):** Since the range and null space are subspaces, they have dimensions. $rank(T) = dim(range(T))$ measures the "dimension of the output", while $nullity(T) = dim(Null(T))$ measures the "dimension of the inputs lost".
* **Rank-Nullity Theorem (Thm 5.2.10):** For $T: V \to W$ ($V$ finite-dim), $rank(T) + nullity(T) = dim(V)$.
    * **Rationale:** This theorem expresses a fundamental conservation principle. The dimensions available in the domain $V$ are perfectly accounted for: some dimension is "preserved" and shows up in the dimension of the range (rank), while the rest is "collapsed" into the dimension of the null space (nullity). The sum is always the original dimension of the input space. This provides a crucial link between the "size" of the domain, range, and null space.

**Rationale for Connecting Null Space/Range to Injectivity/Surjectivity/Solutions:**

* **Injectivity (Prop 5.2.11):** $T$ is injective if and only if $Null(T) = \{\vec{0}_V\}$.
    * **Rationale:** If $T(\vec{v}_1) = T(\vec{v}_2)$, then $T(\vec{v}_1 - \vec{v}_2) = \vec{0}_W$. For $T$ to be injective, this should only happen when $\vec{v}_1 - \vec{v}_2 = \vec{0}_V$. This means the *only* vector that can map to $\vec{0}_W$ is $\vec{0}_V$. The nullity directly quantifies the "failure" of injectivity.
* **Surjectivity:** $T$ is surjective if and only if $range(T) = W$.
    * **Rationale:** This is essentially the definition. Surjectivity means every vector in $W$ is an output. The rank quantifies the "success" of surjectivity; $T$ is surjective iff $rank(T) = dim(W)$.
* **Structure of Solutions to $T(\vec{x}) = \vec{b}$ (Cor 5.2.7):** If $\vec{v}_p$ is one particular solution ($T(\vec{v}_p) = \vec{b}$), then the set of *all* solutions is $\{\vec{v}_p + \vec{z} \,:\, \vec{z} \in Null(T)\}$.
    * **Rationale:** Any two solutions $\vec{x}_1, \vec{x}_2$ to $T(\vec{x})=\vec{b}$ must satisfy $T(\vec{x}_1 - \vec{x}_2) = T(\vec{x}_1) - T(\vec{x}_2) = \vec{b} - \vec{b} = \vec{0}_W$. So, their difference lies in the null space. This means any solution $\vec{x}$ can be written as $\vec{x} = \vec{v}_p + (\vec{x} - \vec{v}_p)$, where $\vec{x} - \vec{v}_p \in Null(T)$. Geometrically, the solution set is a "shifted" version of the null space.

In summary, Section 5.2 defines and analyzes the range and null space because they are fundamental subspaces that reveal key aspects of a linear transformation's behavior – its outputs, what it collapses, its injectivity, and its surjectivity. The Rank-Nullity Theorem provides a crucial link between the dimensions of these spaces and the domain. These concepts are also essential for understanding the structure of solutions to linear systems.

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

**Core Idea: Generalizing Signed Area/Volume and Linking it to Matrix Properties**

Remember back in Section 3.4 we defined the determinant for $2 \times 2$ matrices, $\det\begin{pmatrix} a & b \\ c & d \end{pmatrix} = ad-bc$, and interpreted it as the *signed area* of the parallelogram formed by the column (or row) vectors. Section 5.3 aims to generalize this concept to $n \times n$ matrices. The key goals are:

1.  **Geometric Intuition:** To define a number associated with $n$ vectors in $\mathbb{R}^n$ (or an $n \times n$ matrix) that represents the **signed $n$-dimensional volume** of the parallelepiped they form. The sign should indicate orientation (like right-hand vs. left-hand rule in $\mathbb{R}^3$).
2.  **Algebraic Properties:** To find a function that behaves predictably and has useful algebraic properties, especially concerning matrix operations and invertibility.

**The Rationale - Defining the Determinant Axiomatically (Definition 5.3.1):**

* **Challenge:** Defining "volume" and "orientation" geometrically becomes very difficult and non-intuitive for dimensions $n > 3$.
* **Solution:** Instead of a direct geometric formula, the determinant is defined *axiomatically*. We list the essential properties that a signed $n$-dimensional volume function *should* satisfy:
    1.  **Normalization:** The volume of the standard unit "hypercube" formed by $\vec{e}_1, \dots, \vec{e}_n$ should be 1. ($f(\vec{e}_1, \dots, \vec{e}_n) = 1$).
    2.  **Degeneracy:** If you repeat a vector (i.e., $\vec{v}_i = \vec{v}_j$), the parallelepiped is "flat" in at least one direction and should have zero $n$-dimensional volume. ($f(\dots, \vec{v}, \dots, \vec{v}, \dots) = 0$).
    3.  **Linearity (Scaling):** Scaling one of the vectors by $c$ should scale the signed volume by $c$. ($f(\dots, c\vec{v}_k, \dots) = c \cdot f(\dots, \vec{v}_k, \dots)$). This handles both magnitude scaling and orientation reversal (if $c < 0$).
    4.  **Linearity (Addition):** This property ($f(\dots, \vec{u}+\vec{w}, \dots) = f(\dots, \vec{u}, \dots) + f(\dots, \vec{w}, \dots)$) is less geometrically obvious but is crucial for algebraic manipulation and ensures compatibility with vector addition.
* **Uniqueness (Theorem 5.3.2):** A fundamental (and non-trivial) result is that for any $n$, there exists *exactly one* function satisfying these axioms. This unique function is the determinant, $\det$. This justifies defining the determinant via these properties.

**The Rationale - Connecting Determinants to Row Operations and Properties:**

Defining the determinant of a matrix $A$ as the determinant function applied to its *rows* (Definition 5.3.6) allows us to understand how elementary row operations affect the determinant, based on the axioms:

1.  **Swapping Rows (Prop 5.3.3):** Swapping two rows multiplies the determinant by $-1$.
    * **Rationale:** Follows algebraically from the axioms. Geometrically corresponds to changing the orientation.
2.  **Scaling a Row (Axiom 3):** Multiplying a row by $c$ multiplies the determinant by $c$.
    * **Rationale:** Directly from the scaling property of the determinant function.
3.  **Adding a Multiple of One Row to Another (Prop 5.3.4):** This operation *does not change* the determinant.
    * **Rationale:** Follows algebraically from linearity and the degeneracy property ($f(\dots, \vec{v}_i, \dots, c\vec{v}_i, \dots) = 0$). Geometrically, this corresponds to a "shear" transformation of the parallelepiped, which preserves volume.

**The Rationale - Computational Methods and Key Theorems:**

1.  **Computation via Row Reduction:** The properties above provide a practical method to compute determinants. Use row operations (mostly row combinations, which don't change the determinant, and swaps, which just flip the sign) to reduce the matrix to an upper triangular form. The determinant of a triangular matrix is just the product of the diagonal entries (Prop 5.3.10). Keep track of the sign changes from swaps.
    * **Rationale:** This leverages the efficient Gaussian elimination process and the simple determinant calculation for triangular matrices.
2.  **Cofactor Expansion (Theorem 5.3.14):** Provides a recursive formula to compute determinants.
    * **Rationale:** This formula arises naturally when fully expanding the determinant definition using multilinearity. It connects the determinant of an $n \times n$ matrix to determinants of smaller $(n-1) \times (n-1)$ matrices. While often slower than row reduction for large matrices, it's important theoretically and useful for smaller cases (like $3 \times 3$).
3.  **Determinant and Invertibility (Corollary 5.3.11):** $A$ is invertible $\iff \det(A) \ne 0$.
    * **Rationale:** This is arguably the most important property algebraically. If $\det(A) = 0$, it means the rows are linearly dependent (Prop 5.3.5, Prop 5.3.8), so the matrix can't be row reduced to the identity, hence it's not invertible. Conversely, if $A$ is invertible, its RREF is $I$, and $\det(I)=1 \ne 0$. Since row operations only multiply the determinant by non-zero numbers, $\det(A)$ must have been non-zero. Geometrically, invertibility requires the transformation not to collapse space into a lower dimension, meaning the volume factor ($\det(A)$) must be non-zero.
4.  **Determinant of a Product (Theorem 5.3.15):** $\det(AB) = \det(A) \cdot \det(B)$.
    * **Rationale:** This connects determinants with matrix multiplication (and thus function composition). The volume scaling factor of a composition of transformations is the product of the individual scaling factors.

In essence, Section 5.3 defines the determinant as a function capturing signed volume and satisfying key linearity properties. This function provides a powerful tool linking the geometry of transformations (volume scaling, orientation) with the algebra of matrices (invertibility, row operations) and provides methods for computation.

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

**Core Idea: Finding the "Natural Axes" of a Linear Transformation**

When a linear transformation $T$ maps a vector space $V$ to itself (i.e., $T: V \to V$), we can ask if there are any special vectors whose direction is *unchanged* (or simply reversed) by the transformation. That is, applying $T$ to such a vector only *scales* it, it doesn't rotate it off its original line through the origin. These special vectors and their corresponding scaling factors are the eigenvectors and eigenvalues.

**Rationale for Eigenvalues and Eigenvectors (Definition 5.4.1 / 5.4.3):**

1.  **Geometric Motivation:** Imagine applying a linear transformation $T: \mathbb{R}^2 \to \mathbb{R}^2$. Most vectors will be moved and rotated to point in a different direction from where they started. However, some special vectors $\vec{v}$ might just get stretched or shrunk, so $T(\vec{v})$ is parallel to $\vec{v}$. This means $T(\vec{v}) = \lambda \vec{v}$ for some scalar $\lambda$. These vectors $\vec{v}$ (which must be non-zero by definition) point along the "natural axes" or fundamental directions of the transformation $T$. The scalar $\lambda$ tells us the scaling factor along that direction.
2.  **Why $T: V \to V$?** The equation $T(\vec{v}) = \lambda \vec{v}$ only makes sense if the input $\vec{v}$ and the output $T(\vec{v})$ live in the same vector space $V$.
3.  **Simplifying Transformations:** If we can find a basis consisting entirely of eigenvectors, then the action of $T$ becomes very simple when described relative to that basis – it's just scaling along the basis directions. This was the motivation hinted at in Section 3.2 when a change of basis made the matrix diagonal.

**Rationale for Eigenspace (Proposition 5.4.2):**

* **Definition:** For a given eigenvalue $\lambda$, the eigenspace $E_\lambda$ is the set of *all* vectors $\vec{v}$ (including $\vec{0}$) such that $T(\vec{v}) = \lambda \vec{v}$.
* **Why Study It?** It groups together all vectors that are scaled by the *same* factor $\lambda$.
* **Subspace Property:** Eigenspaces are subspaces of $V$.
    * **Rationale:** This is crucial because it means the set of vectors behaving in this simple way (scaled by $\lambda$) has structure. If $\vec{v}_1$ and $\vec{v}_2$ are scaled by $\lambda$, so is their sum $\vec{v}_1 + \vec{v}_2$ and any scalar multiple $c\vec{v}_1$. This allows us to find a *basis* for the eigenspace, summarizing all eigenvectors for $\lambda$ efficiently.

**Rationale for the Computational Approach (Matrices, Null Spaces, Determinants):**

How do we actually *find* these special vectors and scalars for $T: \mathbb{R}^n \to \mathbb{R}^n$ (represented by matrix $A = [T]$)?

1.  **Connecting to Null Space (Prop 5.4.4):** The core algebraic trick is rewriting the eigenvalue equation:
    $A\vec{v} = \lambda\vec{v} \iff A\vec{v} - \lambda\vec{v} = \vec{0} \iff A\vec{v} - \lambda I \vec{v} = \vec{0} \iff (A - \lambda I)\vec{v} = \vec{0}$.
    * **Rationale:** This converts the eigenvalue problem into finding non-zero vectors in the null space of a *different* matrix, $A - \lambda I$. We already know how to find null spaces using Gaussian elimination.
2.  **Finding Eigenvalues (Corollary 5.4.5 & Definition 5.4.6):**
    * A scalar $\lambda$ is an eigenvalue $\iff$ there exists a non-zero $\vec{v}$ such that $(A - \lambda I)\vec{v} = \vec{0}$.
    * This means $\lambda$ is an eigenvalue $\iff Null(A - \lambda I) \ne \{\vec{0}\}$.
    * For a square matrix $M$, $Null(M) \ne \{\vec{0}\} \iff M$ is not invertible $\iff \det(M) = 0$.
    * Therefore, $\lambda$ is an eigenvalue $\iff \det(A - \lambda I) = 0$.
    * **Rationale:** This gives us a computational method! The expression $\det(A - \lambda I)$ is a polynomial in $\lambda$ (the **characteristic polynomial**). Its roots are precisely the eigenvalues of $A$. Finding eigenvalues is reduced to finding roots of a polynomial.
3.  **Finding Eigenvectors/Eigenspaces:** Once an eigenvalue $\lambda$ is found (by solving $\det(A - \lambda I) = 0$), the corresponding eigenvectors are simply the non-zero vectors in $Null(A - \lambda I)$. The eigenspace is the entire null space $Null(A - \lambda I)$.
    * **Rationale:** This links back to the null space calculation method from Section 4.2 and 5.2 (solving the homogeneous system $(A - \lambda I)\vec{x} = \vec{0}$).

**Rationale for Diagonalization (Definition 5.4.9 & Corollary 5.4.11):**

* **Goal:** To find a basis $\alpha = (\vec{u}_1, \dots, \vec{u}_n)$ consisting entirely of eigenvectors.
* **Why?** If such a basis exists, the matrix $[T]_\alpha^\alpha$ becomes diagonal, with the eigenvalues on the diagonal (Prop 5.4.10).
    * **Rationale:** Relative to this basis, the transformation $T$ is just simple scaling along the basis directions. This makes $T$'s action easy to understand geometrically and computationally (e.g., for calculating powers $A^k = PD^kP^{-1}$).
* **Definition:** A transformation $T$ (or its matrix $A$) is **diagonalizable** if such an eigenbasis exists.
* **Condition:** $T$ is diagonalizable if and only if we can find enough linearly independent eigenvectors to form a basis for the entire vector space $V$. (Having $n$ distinct eigenvalues is sufficient, but not necessary).

In summary, Section 5.4 introduces eigenvalues and eigenvectors as the scaling factors and invariant directions that simplify the understanding of a linear transformation $T: V \to V$. The rationale is to leverage these to understand $T$'s geometry and to simplify computations. The section provides an algebraic pathway (via the characteristic polynomial derived from determinants and the connection to null spaces) to find these eigenvalues and eigenvectors. Diagonalization is presented as the ideal outcome where the transformation becomes simple scaling relative to an eigenbasis.

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



