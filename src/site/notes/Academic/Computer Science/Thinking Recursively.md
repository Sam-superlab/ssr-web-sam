---
{"dg-publish":true,"permalink":"/Academic/Computer Science/Thinking Recursively/"}
---

### Notes on Recursive Thinking (Based on the Document)

---

#### **Recursive Decomposition**:
- Recursive thinking involves breaking down a complex problem into smaller, more manageable sub-problems.
- Example: Creating complex images by first generating smaller components like trees or cottages, then combining them.
- The key idea is to recognize that some problems can be reduced to simpler versions of themselves, which are easier to solve.

---

#### **Recursion in Lists**:
- Lists can be processed recursively by breaking them down into their "head" (first element) and "tail" (the rest of the list).
- In recursive list processing, the list is either:
  - **Empty (base case)**: When the list has no elements, recursion stops.
  - **Non-empty (recursive case)**: Process the first element (head), then recursively process the rest (tail).

---

#### **Example: Summation with Recursion**:
- The `sum` function can be implemented recursively by adding the first element (head) to the sum of the rest (tail).
  - **Base case**: The sum of an empty list is 0.
  - **Recursive case**: The sum of a non-empty list is `head + sum(tail)`.

  ```scheme
  (define sum
    (lambda (numbers)
      (if (null? numbers)
          0
          (+ (car numbers) (sum (cdr numbers))))))
  ```

---

#### **Recursive List Structures**:
- Recursive structures in functional programming allow expressing any non-empty list as:
  - The head element.
  - The rest of the list (which is another list).
- This recursive approach leads to concise solutions for problems like summation, searching, and filtering elements in lists.

---

#### **Functions to Handle Lists Recursively**:
- **`car`**: Returns the first element (head) of a list.
- **`cdr`**: Returns the rest (tail) of the list (everything except the head).
- **`cons`**: Constructs a new list by adding an element to the front of an existing list.

---

#### **Recursive Example: Singleton Check**:
- A function that checks if a list contains exactly one element:
  ```scheme
  (define singleton?
    (lambda (lst)
      (and (not (null? lst))
           (null? (cdr lst)))))
  ```

---

#### **Recursive Example: Summation Walkthrough**:
- The step-by-step process of summing elements recursively involves:
  1. Breaking the list into the head and tail.
  2. Recursively summing the tail.
  3. Adding the head to the result of the recursive sum of the tail.

---

#### **Self-Check Questions**:
1. **Filling in recursive derivation**: Practice tracing the recursive steps of a function.
2. **Understanding infinite recursion**: Avoid common pitfalls like not reducing the problem in each recursive call, which can lead to infinite loops.

---
