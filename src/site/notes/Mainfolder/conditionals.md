---
{"dg-publish":true,"permalink":"/Mainfolder/conditionals/"}
---

### **Overview:**
Conditionals allow a program to make decisions based on the evaluation of boolean expressions. In **Scamper** (a variant of Scheme), conditionals enable you to execute different branches of code depending on whether a boolean expression evaluates to true or false. This is essential for implementing control flow in programs, allowing for dynamic behavior based on different conditions.

The two main forms of conditionals in Scamper are `if` and `cond`. They use **boolean expressions** (which return `#t` for true or `#f` for false) to determine which part of the code should be executed.

---

### **Key Conditional Constructs in Scamper**:

1. **The `if` Expression**:
   - The simplest form of a conditional in Scamper is the `if` expression, which takes three parts: a condition (boolean expression), a branch to evaluate if the condition is true, and a branch to evaluate if the condition is false.
   - **Syntax**:
     ```scheme
     (if <condition>
         <true-branch>
         <false-branch>)
     ```
   - **Example**:
     ```scheme
     (if (> 5 3)
         "True"
         "False")
     ```
     - Here, the condition `> 5 3` evaluates to `#t` (true), so the `true-branch` is executed, resulting in `"True"`.

   **Steps for `if` Evaluation**:
   - First, the condition is evaluated.
   - If the condition evaluates to `#t`, the expression in the true branch is executed.
   - If the condition evaluates to `#f`, the expression in the false branch is executed.

---

2. **The `cond` Expression**:
   - For more complex cases with multiple conditions, you can use the `cond` expression, which allows you to evaluate multiple conditions in sequence and execute the branch of the first true condition.
   - **Syntax**:
     ```scheme
     (cond
       (<condition1> <branch1>)
       (<condition2> <branch2>)
       ...
       (else <default-branch>))
     ```
   - **Example**:
     ```scheme
     (cond
       ((> 5 3) "5 is greater")
       ((= 5 5) "Equal")
       (else "None of the above"))
     ```
     - The first condition `(> 5 3)` is true, so `"5 is greater"` is returned. The rest of the conditions are not evaluated once a true condition is found.

   **Steps for `cond` Evaluation**:
   - Each condition is evaluated in sequence from top to bottom.
   - The first true condition’s branch is executed, and the rest of the branches are ignored.
   - The `else` branch acts as a catch-all if no conditions are true.

---

### **Boolean Expressions**:

Conditionals rely on **boolean expressions** to evaluate to either `#t` or `#f`. These boolean expressions often involve comparison operators or logical operators:

1. **Comparison Operators**:
   - `=`: Checks if two numbers are equal.
   - `>`: Checks if the left number is greater than the right.
   - `<`: Checks if the left number is less than the right.
   - `<=`: Checks if the left number is less than or equal to the right.
   - `>=`: Checks if the left number is greater than or equal to the right.
   - **Example**:
     ```scheme
     (> 10 5)    ; #t
     (= 3 3)     ; #t
     (< 4 2)     ; #f
     ```

2. **Logical Operators**:
   - `and`: Returns `#t` if all arguments are true.
   - `or`: Returns `#t` if at least one argument is true.
   - `not`: Returns `#t` if the argument is false.
   - **Example**:
     ```scheme
     (and (> 5 3) (< 10 20))   ; #t (both conditions are true)
     (or (> 5 3) (< 10 2))     ; #t (at least one condition is true)
     (not (> 5 10))            ; #t (negates the false result)
     ```

---

### **Examples of Using Conditionals in Programs**:

1. **Simple Decision Making with `if`**:
   - This example checks if a number is positive or negative.
   ```scheme
   (define check-number
     (lambda (n)
       (if (> n 0)
           "Positive"
           "Negative or Zero")))
   
   (check-number 5)   ; "Positive"
   (check-number -3)  ; "Negative or Zero"
   ```

2. **Complex Decision Making with `cond`**:
   - This example categorizes a number into positive, negative, or zero.
   ```scheme
   (define categorize-number
     (lambda (n)
       (cond
         ((> n 0) "Positive")
         ((< n 0) "Negative")
         (else "Zero"))))
   
   (categorize-number 5)    ; "Positive"
   (categorize-number -5)   ; "Negative"
   (categorize-number 0)    ; "Zero"
   ```

---

### **Conditional Expressions with Boolean Logic**:

You can combine multiple boolean expressions within conditionals to create more complex decision-making processes.

**Example**:
```scheme
(define is-teenager
  (lambda (age)
    (if (and (>= age 13) (<= age 19))
        "Teenager"
        "Not a Teenager")))

(is-teenager 15)    ; "Teenager"
(is-teenager 22)    ; "Not a Teenager"
```
- In this example, the `if` expression uses the `and` operator to check if the age is between 13 and 19 (inclusive). If both conditions are true, the person is considered a teenager.

---

### **Using Conditionals for Error Handling**:

Conditionals can also be used to handle errors or unexpected inputs in a program.

**Example**:
```scheme
(define divide
  (lambda (a b)
    (if (= b 0)
        "Error: Division by zero"
        (/ a b))))
```
- This `divide` function checks if the divisor `b` is zero. If it is, it returns an error message instead of performing the division. Otherwise, it performs the division.

---

### **Tracing Conditionals**:

1. **Simple `if` Example**:
   ```scheme
   (if (> 7 3)
       (+ 2 2)
       (- 5 1))
   ```
   **Steps**:
   - Evaluate the condition `(> 7 3)` → `#t`.
   - Since the condition is true, evaluate the `true-branch`: `(+ 2 2)` → 4.
   - The `false-branch` is ignored.

2. **Nested `if` Example**:
   ```scheme
   (if (= 10 10)
       (if (> 5 3)
           "Nested True"
           "Nested False")
       "Outer False")
   ```
   **Steps**:
   - First, evaluate the outer `if` condition: `(= 10 10)` → `#t`.
   - Since the outer condition is true, evaluate the inner `if`: `(> 5 3)` → `#t`.
   - Since the inner condition is true, the result is `"Nested True"`.

---

### **Best Practices with Conditionals**:

1. **Use `cond` for Multiple Conditions**:
   - When you have more than two conditions to evaluate, use `cond` instead of chaining multiple `if` statements. This improves readability and avoids unnecessary complexity.
   - **Example**:
     ```scheme
     (cond
       ((> n 0) "Positive")
       ((< n 0) "Negative")
       (else "Zero"))
     ```

2. **Boolean Logic Simplification**:
   - When using boolean operators like `and`, `or`, and `not`, simplify the expressions where possible to make your conditionals more readable.
   - Instead of:
     ```scheme
     (if (and (= a 5) (= b 10))
         "True"
         "False")
     ```
     You could directly return the boolean result:
     ```scheme
     (and (= a 5) (= b 10))
     ```

3. **Handle Edge Cases in Conditionals**:
   - Always ensure that all possible cases are handled in your conditionals, especially when using `cond`. The `else` clause is useful for covering any unexpected or default scenarios.

---

### **Advanced Conditionals with Recursion**:

Conditionals are often used in recursive functions to determine the base case and the recursive case.

**Example: Sum of a List**:
```scheme
(define sum-list
  (lambda (lst)
    (if (null? lst)
        0
        (+ (car lst) (sum-list (cdr lst))))))
```
- The `if` checks if the list is empty (`null? lst`). If it is, the base case returns 0. Otherwise, the function recursively sums the rest of the list.

---

### **Conclusion**:
Conditionals are a fundamental control structure in Scamper that allow your programs to make decisions based on boolean expressions. The use of `if` and `cond` expressions, along with boolean logic, enables you to write dynamic, flexible code that can handle a variety