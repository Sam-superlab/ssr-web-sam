---
{"dg-publish":true,"permalink":"/Mainfolder/Primitive types/"}
---

### **Overview:**
Primitive types are the simplest types of data that a programming language can manipulate directly. In Scamper (a dialect of Scheme), the primary primitive types include **numbers**, **strings**, and **booleans**. These types are the building blocks of all computations, and understanding how to manipulate them using standard functions is essential to solving problems effectively.

By expressing basic computations over these types, you can perform arithmetic operations, string manipulations, and logical comparisons. These operations form the foundation of more complex expressions and functions in Scamper.

---

### **Key Primitive Types in Scamper:**

1. **Numbers**:
   - Numbers in Scamper can be **integers** (whole numbers) or **floating-point numbers** (decimal numbers).
   - **Example**:
     ```scheme
     42    ; Integer
     3.14  ; Floating-point number
     ```

   **Standard Library Functions**:
   - **Arithmetic**:
     - `+`: Adds two or more numbers.
     - `-`: Subtracts one number from another.
     - `*`: Multiplies two or more numbers.
     - `/`: Divides one number by another.
     ```scheme
     (+ 2 3)    ; 5
     (- 5 2)    ; 3
     (* 4 2)    ; 8
     (/ 10 2)   ; 5
     ```

   - **Comparisons**:
     - `<`, `>`, `<=`, `>=`: Compare numbers.
     - `=`: Checks if two numbers are equal.
     ```scheme
     (> 5 3)    ; #t (true)
     (< 3 7)    ; #t
     (= 4 4)    ; #t
     ```

   - **Advanced Operations**:
     - `modulo`: Returns the remainder of the division of two numbers.
     - `expt`: Raises a number to a power.
     ```scheme
     (modulo 10 3)   ; 1
     (expt 2 3)      ; 8
     ```

2. **Strings**:
   - A **string** is a sequence of characters enclosed in double quotes. Strings can represent words, sentences, or any collection of characters.
   - **Example**:
     ```scheme
     "Hello, World!"
     "12345"
     ```

   **Standard Library Functions**:
   - **Concatenation**:
     - `string-append`: Joins two or more strings together.
     ```scheme
     (string-append "Hello, " "World!")   ; "Hello, World!"
     ```

   - **String Length**:
     - `string-length`: Returns the number of characters in a string.
     ```scheme
     (string-length "Hello")   ; 5
     ```

   - **String Comparison**:
     - `string=?`: Compares two strings for equality.
     - `string<?`, `string>?`: Compare strings lexicographically.
     ```scheme
     (string=? "apple" "apple")    ; #t
     (string<? "apple" "banana")   ; #t
     ```

   - **Substring Extraction**:
     - `substring`: Extracts a part of a string.
     ```scheme
     (substring "Functional Programming" 0 11)   ; "Functional"
     ```

3. **Booleans**:
   - Booleans represent **truth values** and are used in conditions and logical expressions. The two boolean values are `#t` (true) and `#f` (false).
   - **Example**:
     ```scheme
     #t    ; True
     #f    ; False
     ```

   **Standard Library Functions**:
   - **Logical Operators**:
     - `and`: Returns `#t` if all arguments are true.
     - `or`: Returns `#t` if at least one argument is true.
     - `not`: Returns `#t` if the argument is false, and vice versa.
     ```scheme
     (and #t #t)    ; #t
     (or #f #t)     ; #t
     (not #t)       ; #f
     ```

   - **Conditional Expressions**:
     - Booleans are often used in `if` and `cond` statements to control the flow of the program.
     ```scheme
     (if (> 5 3)
         "Yes"
         "No")
     ```

---

### **Combining Primitive Types in Expressions**:

1. **Arithmetic with Conditionals**:
   You can combine arithmetic operations with conditionals to create more complex logic.
   **Example**:
   ```scheme
   (define check-number
     (lambda (x)
       (if (> x 0)
           "Positive"
           "Negative or Zero")))
   
   (check-number 5)    ; "Positive"
   ```

2. **String Manipulation**:
   Strings are often used for building messages, combining user input, or outputting results.
   **Example**:
   ```scheme
   (define greeting
     (lambda (name)
       (string-append "Hello, " name "!")))
   
   (greeting "Alice")    ; "Hello, Alice!"
   ```

3. **Boolean Logic in Programs**:
   Booleans are essential for controlling program flow and making decisions based on conditions.
   **Example**:
   ```scheme
   (define is-even
     (lambda (n)
       (if (= (modulo n 2) 0)
           #t
           #f)))
   
   (is-even 4)    ; #t
   (is-even 5)    ; #f
   ```

---

### **Type Checking in Scamper**:

In Scheme, you can check the type of a value using specific type-checking functions. These functions return a boolean indicating whether the value is of the specified type.

**Standard Library Functions for Type Checking**:
1. **Number Check**:
   - `number?`: Checks if a value is a number.
   ```scheme
   (number? 5)     ; #t
   (number? "5")   ; #f
   ```

2. **String Check**:
   - `string?`: Checks if a value is a string.
   ```scheme
   (string? "Hello")    ; #t
   (string? 123)        ; #f
   ```

3. **Boolean Check**:
   - `boolean?`: Checks if a value is a boolean.
   ```scheme
   (boolean? #t)    ; #t
   (boolean? "True")    ; #f
   ```

---

### **Using Primitive Types in Functions**:

1. **Functions with Number Parameters**:
   Many functions take numbers as inputs, perform arithmetic or logical operations, and return results.
   **Example**:
   ```scheme
   (define add-two
     (lambda (x y)
       (+ x y)))
   
   (add-two 3 5)    ; 8
   ```

2. **Functions with String Parameters**:
   String-based functions often manipulate text, such as formatting or concatenating strings.
   **Example**:
   ```scheme
   (define format-message
     (lambda (name score)
       (string-append name " scored " (number->string score) " points!")))
   
   (format-message "Alice" 100)    ; "Alice scored 100 points!"
   ```

3. **Functions with Boolean Parameters**:
   Functions that accept booleans typically involve conditional logic, where decisions are made based on the truth value of the input.
   **Example**:
   ```scheme
   (define check-valid
     (lambda (flag)
       (if flag
           "Valid"
           "Invalid")))
   
   (check-valid #t)    ; "Valid"
   ```

---

### **Practical Applications of Primitive Types**:

1. **User Input and Output**:
   - Numbers, strings, and booleans are used to process user input and format output. For example, a program may ask for a user’s age (number) and respond with a message (string) based on whether they are an adult (boolean).

2. **Data Validation**:
   - Booleans are commonly used to validate data. A boolean function can check if an input is valid, and based on that validation, the program can proceed or return an error.

3. **Mathematical and Financial Calculations**:
   - Numbers are used extensively in programs that involve mathematical or financial calculations, such as determining totals, averages, or differences between values.

4. **String Manipulation in Text Processing**:
   - In programs that deal with text, strings are used to format and manipulate data. For example, you can build sentences dynamically or extract key information from a large text.

---

### **Conclusion**:
Primitive types—numbers, strings, and booleans—are the fundamental building blocks of programming in Scamper. Mastering the use of these types, along with their associated standard library functions, allows you to perform a wide range of basic computations. Whether you’re performing arithmetic, manipulating strings, or evaluating logical expressions, these types are essential for constructing more complex programs.