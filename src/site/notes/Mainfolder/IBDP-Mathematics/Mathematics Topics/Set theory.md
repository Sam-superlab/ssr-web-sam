---
{"dg-publish":true,"permalink":"/Mainfolder/IBDP-Mathematics/Mathematics Topics/Set theory/"}
---

# Introduction to Set Theory

## Basic Definitions

### Set, Element, Subset
- **Set**: A set is a well-defined collection of distinct objects, considered as an object in its own right. The objects in a set are called **elements** or **members** of the set.
- **Element**: If $a$ is an object, we say $a$ is an **element** of a set $A$ if $a$ belongs to the set. This is denoted as $a \in A$.
- **Subset**: A set $A$ is called a **subset** of another set $B$ if every element of $A$ is also an element of $B$. This is denoted as $A \subseteq B$.

### Example:
Let $A = \{1, 2, 3\}$ and $B = \{1, 2, 3, 4, 5\}$. Since every element of $A$ is also in $B$, we say $A$ is a subset of $B$: $A \subseteq B$.

### Empty Set
- **Empty Set**: The **empty set**, denoted by $\emptyset$, is the set that contains no elements. Formally:
$$
\emptyset = \{\}
$$

### Universal Set
- **Universal Set**: The **universal set** is the set that contains all possible elements for a particular discussion. It is typically denoted as $U$. All other sets are considered subsets of the universal set.

---

## Set Notation

### Roster Notation
- **Roster Notation**: A set is defined by explicitly listing all of its elements inside curly braces.
  - Example: $A = \{1, 2, 3, 4\}$ means that $A$ is the set containing the elements 1, 2, 3, and 4.

### Set-Builder Notation
- **Set-Builder Notation**: A set is defined by specifying a property that its members must satisfy.
  - Example: $A = \{x \mid x \text{ is an even number}\}$ defines the set $A$ as all even numbers.

---

## Membership and Inclusion

### Membership
- **Membership** is the relationship between an element and a set. If $a$ is an element of a set $A$, we say $a$ **belongs** to $A$ and write:
$$
a \in A
$$
If $a$ does not belong to $A$, we write:
$$
a \notin A
$$

### Subset and Inclusion
- **Subset**: A set $A$ is a subset of another set $B$ if every element of $A$ is also an element of $B$. This is denoted as:
$$
A \subseteq B
$$
- **Proper Subset**: $A$ is a proper subset of $B$, written $A \subset B$, if $A$ is a subset of $B$ but $A \neq B$.

### Example:
If $A = \{1, 2\}$ and $B = \{1, 2, 3\}$, then $A \subseteq B$ because all elements of $A$ are in $B$. However, $A \neq B$, so $A \subset B$ (proper subset).

---

## Venn Diagrams

- **Venn Diagrams**: A Venn diagram visually represents sets and their relationships. Each set is shown as a circle, and the relationships between the sets (such as intersections or unions) are depicted by the overlapping or non-overlapping areas of the circles.

### Common Venn Diagram Operations:
- **Intersection** ($A \cap B$): The set of elements common to both $A$ and $B$. Represented by the overlapping region of two circles.
- **Union** ($A \cup B$): The set of elements that belong to either $A$ or $B$. Represented by the entire area covered by both circles.
- **Complement** ($A^c$): The set of elements not in $A$, but in the universal set $U$.
- **Difference** ($A - B$): The set of elements in $A$ but not in $B$.

### Example:
If $A = \{1, 2, 3\}$ and $B = \{3, 4, 5\}$:
- $A \cup B = \{1, 2, 3, 4, 5\}$ (union)
- $A \cap B = \{3\}$ (intersection)
- $A - B = \{1, 2\}$ (difference)

Venn diagrams provide an intuitive way to visualize these set operations.
