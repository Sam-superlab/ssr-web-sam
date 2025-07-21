---
{"dg-publish":true,"permalink":"/Academic/Mathematics/General vector space/"}
---


# Beyond Two Dimensions

## Section 4.1: Vector Spaces and Subspaces

* **Core Idea:** This section establishes the fundamental "universe" or type of structure (a **Vector Space**) where the concepts of linear algebra primarily operate. It then defines well-behaved subsets (**Subspaces**) within these universes.
* **Rationale for Vector Space (Definition 4.1.1):**
    * **Abstraction and Generality:** The goal is to identify the essential algebraic properties shared by many different mathematical settings where you can meaningfully "add" things and "scale" them by real numbers. Examples include familiar arrows in $\mathbb{R}^n$, but also functions, matrices, sequences, and even more abstract examples. By defining an abstract structure based on common rules (the 10 axioms), we can prove theorems *once* for all vector spaces, rather than re-proving similar results for $\mathbb{R}^n$, then for functions, then for matrices, etc. This reveals deep connections and saves work.
    * **Focus on Operations:** The definition emphasizes the *operations* (addition and scalar multiplication) and the *rules* they follow (the axioms like commutativity, associativity, distributivity, existence of identities and inverses), rather than the specific *nature* of the objects ("vectors") themselves. A vector space is fundamentally a set where linear combinations make sense and behave nicely.
* **Rationale for Subspace (Definition 4.1.12):**
    * **Identifying Vector Spaces Within Vector Spaces:** Often, we are interested in a subset $W$ of a known vector space $V$ (e.g., a plane $W$ within $\mathbb{R}^3$, or continuous functions $W$ within all functions $V$). The question is: when does this subset $W$, using the *same* addition and scalar multiplication inherited from $V$, also qualify as a vector space in its own right?
    * **Inherited Axioms vs. Closure:** Many axioms (like commutativity) are automatically inherited by $W$ because they hold true in the larger space $V$. The crucial properties that might fail are:
        1.  **Closure under Addition:** Is $\vec{w}_1 + \vec{w}_2$ guaranteed to be back in $W$ whenever $\vec{w}_1, \vec{w}_2 \in W$?
        2.  **Closure under Scalar Multiplication:** Is $c \cdot \vec{w}$ guaranteed to be back in $W$ whenever $\vec{w} \in W$ and $c \in \mathbb{R}$?
        3.  **Contains Zero Vector:** Does $W$ contain the additive identity $\vec{0}$ from $V$?
    * **The Definition:** A subspace is defined precisely by these three essential properties. If a subset $W$ satisfies these, all other vector space axioms will hold automatically (including the existence of additive inverses within $W$).
    * **Significance:** Subspaces allow us to study "flat" objects (like lines and planes through the origin in $\mathbb{R}^n$) and other structured subsets (like continuous functions) using the tools of linear algebra. Proposition 4.1.16 is key because it shows that the *span* of any set of vectors is always a subspace, giving a primary method for constructing subspaces.

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
>3. $0 \cdot \vec{v} = \vec{0}$ for all $\vec{v} \in V$
>4. $c \cdot \vec{0} = \vec{0}$ for all $c \in \mathbb{R}$
>5. $(-1) \cdot \vec{v} = -\vec{v}$ for all $\vec{v} \in V$

>[!theorem] Proposition 4.1.16
>Let $V$ be a vector space and let $\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n \in V$. The set $Span(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ is a subspace of $V$

## Section 4.2: Solving Linear Systems

* **Core Idea:** This section develops the fundamental algorithm, **Gaussian Elimination**, for analyzing and solving systems of linear equations.
* **Rationale for Focusing on Linear Systems:**
    * **Central Tool:** Many core questions in linear algebra (Is $\vec{v}$ in $Span(\vec{u}_1, \dots, \vec{u}_n)$? Is $(\vec{u}_1, \dots, \vec{u}_n)$ linearly independent? What are the coordinates $[\vec{v}]_\alpha$?) boil down to solving a system of linear equations. Having a robust method to solve these systems is therefore essential.
    * **Structure and Algorithms:** Linear systems possess a highly regular structure involving only sums of variables multiplied by constants. This regularity allows for the development of systematic, step-by-step algorithms like Gaussian elimination.
* **Rationale for Augmented Matrix (Definition 4.2.7):**
    * **Conciseness:** Writing out variables ($x_1, x_2, \dots$) repeatedly is tedious and unnecessary. The coefficients and the constant terms on the right-hand side contain all the vital information.
    * **Organization:** The matrix format $[A | \vec{b}]$ neatly organizes this information and allows row operations to be performed systematically on the numbers without rewriting variables.
* **Rationale for Elementary Row Operations (Definition 4.2.3):**
    * **Goal:** To transform a complicated system into a simpler, equivalent one (having the same solution set).
    * **Why These Three?**
        1.  They are **reversible** (Prop 4.2.4). This is critical because it guarantees that we don't change the solution set when applying them (Corollary 4.2.5). We can always get back to the original system.
        2.  They are **sufficient** to simplify any system into a standard "staircase" form (echelon form) where the solutions become easier to see.
* **Rationale for Echelon Form (Definition 4.2.9 & 4.2.13):**
    * **Systematic Goal:** Gaussian elimination aims to reach an **echelon form**. This form makes the structure of the solutions apparent.
    * **Easy Solving:** From echelon form, solutions can be found easily via **back-substitution**.
    * **Reduced Echelon Form:** Going further to **reduced echelon form** (where leading entries are 1 and are the only non-zero entry in their column) makes the solutions even more explicit, often requiring little to no algebra during back-substitution.
* **Rationale for Proposition 4.2.12 (Interpreting Echelon Form):**
    * **Connecting Form to Solutions:** This proposition directly links the visual pattern of the echelon form of the *augmented* matrix to the nature of the solution set (no solutions, unique solution, or infinitely many solutions) without needing to fully solve via back-substitution.
    * **Inconsistency:** A leading entry in the *augmented* column (the rightmost one) signals an impossible equation like $0=c$ where $c \ne 0$.
    * **Consistency & Free Variables:** If there's no inconsistency, the existence of columns *without* leading entries (corresponding to variables not solved for at the start of back-substitution) indicates the presence of *free variables*, which can be parameterized to generate infinite solutions. If every variable column has a leading entry, there are no free variables, yielding a unique solution.

In essence, Section 4.1 defines the abstract playing field (Vector Spaces) and important regions within it (Subspaces). Section 4.2 provides the essential computational toolkit (Gaussian Elimination on matrices) for answering concrete questions that arise when working within these abstract structures.

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
**Core Question of Section 4.4:**

Section 4.3 asked: "Can we reach *everything* in the space?" Section 4.4 tackles the complementary question: "Do we have *redundancy* in our list of vectors?" In other words, is there a vector in our sequence $(\vec{u}_1, \vec{u}_2, \dots, \vec{u}_n)$ that is "unnecessary" because it can already be created by combining the others?

**The Initial Idea of Redundancy:**

The most direct way to think about redundancy is to ask if any vector $\vec{u}_k$ in the sequence is a linear combination of the *other* vectors in the sequence, i.e., is $\vec{u}_k \in Span(\vec{u}_1, \dots, \vec{u}_{k-1}, \vec{u}_{k+1}, \dots, \vec{u}_n)$?

**The Problem with the Initial Idea:**

While intuitive, checking this directly is computationally inefficient. For a sequence of $n$ vectors, you would potentially need to set up and solve $n$ different linear systems (one for each vector $\vec{u}_k$ to see if it's in the span of the others).

**The Rationale - A More Elegant Perspective:**

1.  **Rewriting Redundancy:** Suppose a vector $\vec{u}_k$ *is* redundant. This means we can write $\vec{u}_k = c_1\vec{u}_1 + \dots + c_{k-1}\vec{u}_{k-1} + c_{k+1}\vec{u}_{k+1} + \dots + c_n\vec{u}_n$.
2.  **The Homogeneous Equation:** By simply moving $\vec{u}_k$ to the other side, we get:
    $c_1\vec{u}_1 + \dots + c_{k-1}\vec{u}_{k-1} - 1\cdot\vec{u}_k + c_{k+1}\vec{u}_{k+1} + \dots + c_n\vec{u}_n = \vec{0}$.
    Notice this is a linear combination of *all* the vectors $(\vec{u}_1, \dots, \vec{u}_n)$ that equals the zero vector $\vec{0}$. Crucially, at least one coefficient (the $-1$ in front of $\vec{u}_k$) is **nonzero**.
3.  **Linear Dependence:** This motivates the definition. A sequence $(\vec{u}_1, \dots, \vec{u}_n)$ is called **linearly dependent** if there exist scalars $c_1, \dots, c_n$, **not all zero**, such that $c_1\vec{u}_1 + c_2\vec{u}_2 + \dots + c_n\vec{u}_n = \vec{0}$. This condition signals redundancy.
4.  **Linear Independence:** Conversely, the sequence is **linearly independent** if the *only* way to make the linear combination $c_1\vec{u}_1 + c_2\vec{u}_2 + \dots + c_n\vec{u}_n = \vec{0}$ is by choosing the **trivial solution** where $c_1 = c_2 = \dots = c_n = 0$. This means there's no redundancy – no vector can be expressed in terms of the others (Proposition 4.4.2 proves this equivalence formally).

**The Rationale - Connecting Linear Independence to Linear Systems:**

How do we check if the *only* solution to $c_1\vec{u}_1 + c_2\vec{u}_2 + \dots + c_n\vec{u}_n = \vec{0}$ is the trivial one $c_1 = \dots = c_n = 0$?

1.  **Homogeneous System:** This is equivalent to asking if the **homogeneous linear system** $A\vec{c} = \vec{0}$ has *only* the trivial solution $\vec{c} = \vec{0}$, where $A$ is the matrix whose columns are $\vec{u}_1, \dots, \vec{u}_n$.
2.  **Gaussian Elimination Again:** We use Gaussian elimination on the coefficient matrix $A$ (we can ignore the augmented column of zeros as it never changes). Let $B$ be an echelon form of $A$.
3.  **Condition for Trivial Solution Only:** The homogeneous system $A\vec{c} = \vec{0}$ (which has the same solution set as $B\vec{c} = \vec{0}$) has *only* the trivial solution if and only if there are *no free variables*.
4.  **The Key Insight (Proposition 4.4.5):** This happens *exactly when* the echelon form $B$ has a **leading entry (pivot) in every column**. If there's a column without a pivot, that corresponds to a free variable, allowing for non-trivial solutions (meaning linear *dependence*). If every column has a pivot, there are no free variables, forcing the only solution to be the trivial one (meaning linear *independence*).

**Rationale behind the Corollaries:**

* **Corollary 4.4.6:** If $(\vec{u}_1, \dots, \vec{u}_n)$ in $\mathbb{R}^m$ is linearly independent, then $n \le m$.
    * **Rationale:** If the sequence is LI, the echelon form $B$ of $A=[\vec{u}_1|\dots|\vec{u}_n]$ must have a pivot in every column (by Prop 4.4.5). There are $n$ columns, so there are $n$ pivots. Since each row can contain at most one pivot, you need at least $n$ rows to accommodate $n$ pivots. Thus, $m$ (the number of rows) must be $\ge n$. Intuitively, you can't have more independent "directions" (vectors) than the number of dimensions ($m$) of the space they live in.
* **Corollary 4.4.7:** If $n > m$, then $(\vec{u}_1, \dots, \vec{u}_n)$ in $\mathbb{R}^m$ is linearly dependent.
    * **Rationale:** This is the contrapositive of Cor 4.4.6. If you have more vectors ($n$) than the dimension of the space ($m$), they *must* be linearly dependent. An $m \times n$ matrix with $n > m$ cannot have a pivot in every column (since there are at most $m$ pivots total, one per row), so there must be free variables when solving $A\vec{c}=\vec{0}$, guaranteeing non-trivial solutions. Intuitively, if you try to cram too many vectors into a lower-dimensional space, some must become redundant combinations of others.

In summary, Section 4.4 defines linear independence as the absence of non-trivial relationships between vectors (meaning no redundancy). It connects this concept to checking if a homogeneous system $A\vec{c}=\vec{0}$ has only the trivial solution. Gaussian elimination provides the tool (checking for a pivot in every column of the echelon form) to answer this efficiently. The corollaries establish fundamental limits on the number of linearly independent vectors based on the dimension of the ambient space.

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


**Core Idea of Section 4.5: Finding the "Right" Set of Vectors**

The goal is to identify the most "efficient" set of vectors to describe a vector space $V$. What does efficient mean here?

1.  **Sufficiency (Spanning):** The set must be large enough so that linear combinations of its vectors can create *every* vector in the space $V$. This is the idea of a **spanning sequence** from Section 4.3. We need $Span(\vec{u}_1, \dots, \vec{u}_n) = V$.
2.  **No Redundancy (Linear Independence):** The set should be "minimal" in the sense that it doesn't contain unnecessary vectors. If we can create one vector in the set using the others, it's redundant. This is precisely the idea captured by **linear independence** from Section 4.4. We need $(\vec{u}_1, \dots, \vec{u}_n)$ to be linearly independent.

**Rationale for "Basis" (Definition 4.5.1)**

A **basis** is defined as a sequence of vectors $(\vec{u}_1, \dots, \vec{u}_n)$ that satisfies *both* of the above conditions:
1.  It spans the entire space $V$.
2.  It is linearly independent.

* **Rationale:** A basis hits the "sweet spot". It contains enough vectors to generate everything (it spans $V$), but it's lean enough that it contains no redundant information (it's linearly independent). It's the smallest possible set of vectors that can still generate the whole space.

**Rationale for Theorem 4.5.2 (Basis $\iff$ Unique Representation)**

This theorem provides the crucial insight into *why* bases are so fundamental:

* **Statement:** A sequence $\alpha = (\vec{u}_1, \dots, \vec{u}_n)$ is a basis for $V$ if and only if every vector $\vec{v} \in V$ can be written as a linear combination $\vec{v} = c_1\vec{u}_1 + \dots + c_n\vec{u}_n$ in **exactly one way** (i.e., the scalars $c_1, \dots, c_n$ are unique for each $\vec{v}$).
* **Rationale:**
    * The **spanning** property guarantees *existence* – that for any $\vec{v}$, there is at least one way to write it as a linear combination.
    * The **linear independence** property guarantees *uniqueness*. If there were two different ways to write $\vec{v}$, subtracting them would give a non-trivial linear combination of the basis vectors that equals $\vec{0}$, which contradicts linear independence.
    * **Significance:** This uniqueness is powerful. It means that once we fix a basis $\alpha$, we can unambiguously associate any vector $\vec{v}$ in our (potentially abstract) vector space $V$ with a specific list of $n$ real numbers $(c_1, \dots, c_n)$.

**Rationale for "Coordinates" (Definition 4.5.3)**

Since Theorem 4.5.2 guarantees a unique list of scalars $c_1, \dots, c_n$ for each $\vec{v}$ relative to a basis $\alpha = (\vec{u}_1, \dots, \vec{u}_n)$, we give this list a name:

* **Definition:** The **coordinates of $\vec{v}$ relative to $\alpha$** is the vector in $\mathbb{R}^n$ formed by these unique scalars: $Coord_\alpha(\vec{v}) = [\vec{v}]_\alpha = \begin{pmatrix} c_1 \\ \vdots \\ c_n \end{pmatrix}$.
* **Rationale:** The $Coord_\alpha$ function acts as a **bridge** or **translator**. It maps vectors in the potentially abstract space $V$ to concrete vectors in $\mathbb{R}^n$. This allows us to translate problems about $V$ into problems about $\mathbb{R}^n$, where we can use familiar tools like matrices and Gaussian elimination. It essentially imposes a coordinate system (like graph paper) onto $V$, using the basis vectors as the axes.

**Rationale for Propositions 4.5.5 and 4.5.6 (Constructing Bases)**

These results provide ways to find a basis:

* **Proposition 4.5.5:** Any finite sequence that spans $V$ can be "trimmed down" by removing redundant vectors until a basis is obtained.
    * **Rationale:** If a spanning set is linearly dependent, it contains redundancy (Prop 4.4.2). We can remove a redundant vector without changing the span (Prop 4.5.4). We repeat this until the set becomes linearly independent, at which point it's a basis because it still spans.
* **Proposition 4.5.6:** Provides a specific algorithm for doing this trimming process for vectors in $\mathbb{R}^m$ whose span is $Col(A)$. It uses Gaussian elimination to identify the redundant columns (those without pivots) and tells us to keep the *original* columns that correspond to pivot columns in the echelon form.
    * **Rationale:** This works because row operations preserve the linear dependency relationships among the columns. The pivot columns of the echelon form are clearly linearly independent, and all other columns are combinations of them. This structure reflects the dependencies in the original columns.

In short, Section 4.5 defines the crucial concept of a basis as the optimal blend of spanning and linear independence. The core rationale is that a basis allows every vector in the space to be represented uniquely by a set of coordinates, effectively translating abstract vector space problems into the concrete setting of $\mathbb{R}^n$. The section also provides methods for constructing a basis from a spanning set.

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
**Core Idea of Section 4.6: Defining the "Size" of a Vector Space**

After establishing bases (Section 4.5) as "efficient" sets that both span the space and have no redundancy (linear independence), a natural question arises: Does every basis for a given vector space $V$ have the same number of elements? Section 4.6 answers this question affirmatively and uses it to define the **dimension** of the space.

**The Rationale - Why Dimension is Well-Defined:**

1.  **The Problem:** Vector spaces can have many different bases. For the concept of "dimension" to be meaningful as an intrinsic property of the space itself, we need to know that the number of vectors in a basis doesn't depend on *which* basis we happen to choose.
2.  **Key Result (Theorem 4.6.2):** This theorem is the cornerstone. It states that if a vector space $V$ can be spanned by $n$ vectors $(\vec{u}_1, \dots, \vec{u}_n)$, then any sequence $(\vec{w}_1, \dots, \vec{w}_m)$ with more than $n$ vectors (i.e., $m > n$) *must* be linearly dependent.
    * **Rationale behind Thm 4.6.2:** The proof uses the **Steinitz Exchange Lemma (Proposition 4.6.1)** repeatedly. The idea is that you can systematically replace vectors in the spanning set $(\vec{u}_i)$ with vectors from the linearly independent set $(\vec{w}_j)$ while maintaining the span. Since you start with only $n$ vectors spanning the space, you can swap in at most $n$ of the $\vec{w}_j$'s. If you have more than $n$ vectors in the $\vec{w}$ sequence ($m > n$), then by the time you consider $\vec{w}_{n+1}$, it *must* be expressible as a linear combination of the preceding $\vec{w}_1, \dots, \vec{w}_n$ (which now span the space), proving the sequence $(\vec{w}_1, \dots, \vec{w}_m)$ is linearly dependent.
3.  **Consequence (Corollary 4.6.3):** Taking the contrapositive of Theorem 4.6.2, we get: If a space $V$ is spanned by $(\vec{u}_1, \dots, \vec{u}_n)$ and $(\vec{w}_1, \dots, \vec{w}_m)$ is linearly independent in $V$, then $m \le n$. In words: the size of any linearly independent set is less than or equal to the size of any spanning set.
4.  **Invariance of Basis Size (Corollary 4.6.4):** This directly uses the previous corollary. If you have two bases, $\alpha$ with $n$ vectors and $\beta$ with $m$ vectors:
    * Since $\alpha$ spans and $\beta$ is linearly independent, $m \le n$.
    * Since $\beta$ spans and $\alpha$ is linearly independent, $n \le m$.
    * Therefore, $m = n$.
5.  **Definition of Dimension (Definition 4.6.5):** Because Corollary 4.6.4 guarantees that *all* bases for a given vector space $V$ (if any exist) have the same number of elements, we can unambiguously define the **dimension** of $V$, denoted $dim(V)$, as this common number.
    * **Rationale:** Dimension captures the intrinsic "size" or number of "degrees of freedom" or independent "directions" within the vector space, regardless of the specific basis chosen to measure it.

**The Rationale - Consequences and Uses of Dimension:**

Once dimension is well-defined, it becomes a powerful tool:

1.  **Basis Shortcut (Proposition 4.6.7):** If you know $dim(V) = n$, then checking if a sequence of exactly $n$ vectors $(\vec{u}_1, \dots, \vec{u}_n)$ is a basis becomes easier. You only need to check *one* of the two conditions:
    * If it's linearly independent, it *must* also span $V$.
    * If it spans $V$, it *must* also be linearly independent.
    * **Rationale:** This follows from Theorem 4.6.2 and its corollary. For instance, if you have $n$ linearly independent vectors, but they didn't span $V$, you could add another vector $\vec{w} \notin Span(\vec{u}_1, \dots, \vec{u}_n)$ to get $n+1$ linearly independent vectors (Prop 4.6.9), which contradicts the fact that the $n$-dimensional space $V$ cannot contain $n+1$ linearly independent vectors (Cor 4.6.3). A similar argument works the other way.
2.  **Subspace Dimension (Proposition 4.6.8):** Any subspace $W$ of a finite-dimensional vector space $V$ is also finite-dimensional, and $dim(W) \le dim(V)$.
    * **Rationale:** You can construct a basis for $W$ by starting with a linearly independent set in $W$ and extending it (using Prop 4.6.10, below). This process must stop because $W$ is contained in $V$, and you can't have more linearly independent vectors in $W$ than the dimension of $V$. This guarantees $W$ has a finite basis, and the number of vectors must be less than or equal to $dim(V)$.
3.  **Extending Linearly Independent Sets (Proposition 4.6.10):** Any linearly independent sequence in a finite-dimensional vector space can be extended to form a basis for that space.
    * **Rationale:** Start with the linearly independent set. If it doesn't already span the whole space, find a vector not in its span and add it to the set; the new set remains linearly independent (Prop 4.6.9). Repeat this process. Since the dimension is finite, you can't keep adding vectors indefinitely while maintaining linear independence (by Thm 4.6.2). The process must stop when the set spans the space, at which point it is a basis. This confirms that linearly independent sets act as valid starting points or "skeletons" for building bases.

In summary, Section 4.6 leverages the interplay between spanning sets and linearly independent sets (specifically Theorem 4.6.2) to rigorously establish that the size of a basis is an invariant property of a vector space, allowing the definition of **dimension**. Dimension then becomes a key characteristic used to understand the structure of the space, relationships between spaces and subspaces, and provides useful criteria for determining if a set of vectors forms a basis.

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
