---
{"dg-publish":true,"permalink":"/Academic/Computer Science/Lists/"}
---

- [[Academic/Computer Science/Lists#**List Basics Overview**:\|**List Basics Overview**:]]
- [[Academic/Computer Science/Lists#**Five Basic Concepts for a New Data Type**:\|**Five Basic Concepts for a New Data Type**:]]
- [[Academic/Computer Science/Lists#**Displaying Lists**:\|**Displaying Lists**:]]
- [[Academic/Computer Science/Lists#**Creating Lists**:\|**Creating Lists**:]]
- [[Academic/Computer Science/Lists#**Common List Operations**:\|**Common List Operations**:]]
- [[Academic/Computer Science/Lists#**List Transformations Overview**:\|**List Transformations Overview**:]]
- [[#**Transformation through `map`**:|**Transformation through `map`**:]]
- [[Academic/Computer Science/Lists#**Transformation Flexibility**:\|**Transformation Flexibility**:]]
- [[Academic/Computer Science/Lists#**Transforming Other Types of Data**:\|**Transforming Other Types of Data**:]]
- [[Academic/Computer Science/Lists#**Errors and Type Matching**:\|**Errors and Type Matching**:]]
- [[#**Using `apply`**:|**Using `apply`**:]]
- [[Academic/Computer Science/Lists#**Dealing with Complex Data**:\|**Dealing with Complex Data**:]]
- [[#**Error Handling in `map` and `apply`**:|**Error Handling in `map` and `apply`**:]]
- [[Academic/Computer Science/Lists#**Summary**:\|**Summary**:]]

### **List Basics Overview**:
In Scheme (and Scamper), a **list** is a fundamental data structure that holds collections of values. Lists are essential for handling multiple data points at once, making them especially useful in more complex problems, such as those found in data science.

The document introduces the basic concepts of **lists** in Scheme, how to create lists, and the operations that can be performed on them.

---

### **Five Basic Concepts for a New Data Type**:

1. **Name**: The data type is called a **list**.
2. **Purpose**: The main purpose of a list is to **group or collect values**.
3. **How to Express Values**: You can create and manipulate lists using specific functions.
4. **Displaying Values**: Lists are displayed either as **function calls** (in Scamper) or as **parenthesized lists** in Scheme.
5. **Operations Available**: A variety of functions can be used to manipulate and build lists.

---

### **Displaying Lists**:

- Lists are created using the **`list` function**. For example:
  ```scheme
  (list 2 12 32)
  ```
  This will create a list with the values `2`, `12`, and `32`.
  
- Example of converting a string to a list:
  ```scheme
  (string->list "hello world!")
  ```
  This converts the string into a list of individual characters: 
  ```scheme
  (#\h #\e #\l #\l #\o #\space #\w #\o #\r #\l #\d #\!)
  ```

---

### **Creating Lists**:

- **Using the `list` function**: 
  ```scheme
  (list (+ 1 1) (string-length "hello world!") 32)
  ```
  This will create a list with the results of expressions: `2`, `12`, and `32`.

- **`make-list` function**: 
  Creates a list of identical values:
  ```scheme
  (make-list 5 "hello")
  ```
  This produces a list with five "hello" strings: 
  ```scheme
  ("hello" "hello" "hello" "hello" "hello")
  ```

- **`range` function**: 
  Produces a list of numbers. It can take one, two, or three arguments to control the start, end, and step of the range:
  ```scheme
  (range 7)        ; produces (0 1 2 3 4 5 6)
  (range 1 10 2)   ; produces (1 3 5 7 9)
  (range 13 -5 -3) ; produces (13 10 7 4 1 -2)
  ```

---

### **Common List Operations**:

1. **`length`**: Returns the number of elements in the list:
   ```scheme
   (length (list 3 4 5)) ; produces 3
   ```

2. **`list-ref`**: Accesses an element of the list at a given index (0-based):
   ```scheme
   (list-ref (list 1 2 3 4) 2) ; produces 3
   ```

3. **`index-of`**: Returns the position of the first occurrence of a value in a list:
   ```scheme
   (index-of (list "a" "b" "c") "b") ; produces 1
   ```

4. **`reverse`**: Reverses the list:
   ```scheme
   (reverse (list 1 2 3 4 5)) ; produces (5 4 3 2 1)
   ```

5. **`append`**: Combines two lists into one:
   ```scheme
   (append (list 1 2) (list 3 4)) ; produces (1 2 3 4)
   ```

6. **`list-take` and `list-drop`**:
   - **`list-take`**: Takes the first n elements from a list.
     ```scheme
     (list-take (list 1 2 3 4 5) 3) ; produces (1 2 3)
     ```
   - **`list-drop`**: Drops the first n elements from a list.
     ```scheme
     (list-drop (list 1 2 3 4 5) 2) ; produces (3 4 5)
     ```

Lists in Scheme provide a versatile way to group and manage data. You can create lists with a wide variety of functions, manipulate them with operations like `append`, `reverse`, `list-ref`, and more, and use them to handle sequences of data efficiently.


### **List Transformations Overview**:
In computing, **list transformations** involve transforming individual elements of a collection, which can be efficiently done using higher-order functions like **`map`** and **`apply`**. This document explains how transformations over collections (lists) are central to functional programming and how they can be performed in Scheme.

---

### **Transformation through `map`**:

The **`map` function** is a higher-order function in Scheme that transforms each element of a list by applying a given function to every element. It takes two arguments:
1. A function that transforms a single element.
2. A list of elements to transform.

For example, if you have a function that adjusts salaries based on a cost-of-living adjustment (COLA):
```scheme
(define compute-cola-salary
  (lambda (salary)
    (+ salary (* salary 0.016))))
```
You can use **`map`** to apply this function to a list of salaries:
```scheme
(map compute-cola-salary (list 100000 100000 50000 75000 500000))
```
This produces:
```scheme
(list 101600 101600 50800 76200 508000)
```

### **Transformation Flexibility**:
- The **`map` function** does not affect the original list. Instead, it generates a new list with transformed elements.
- You can use **`map`** to apply any function, for example, doubling salaries:
  ```scheme
  (define double-salary
    (lambda (salary)
      (* salary 2)))
  (map double-salary salaries) ; produces (200000 200000 100000 150000 1000000)
  ```

### **Transforming Other Types of Data**:
**`map`** can transform any collection, not just numbers. For example:
- To convert a list of strings to uppercase:
  ```scheme
  (map string-upcase (list "please" "be" "quiet" "not" "loud")) 
  ; produces ("PLEASE" "BE" "QUIET" "NOT" "LOUD")
  ```

### **Errors and Type Matching**:
- When using **`map`**, the types of elements in the list must match the type expected by the function. For example, applying `square` to a list of strings will result in an error because `square` expects numbers.
  ```scheme
  (map square (list "please" "be" "quiet")) ; produces a type error
  ```

---

### **Using `apply`**:
While **`map`** applies a function to each element of a list, **`apply`** takes a procedure and applies it to an entire list of arguments at once. 

- Example of using `apply` to sum a list of numbers:
  ```scheme
  (apply + (list 1 2 3 4 5)) ; produces 15
  ```
- Similarly, you can use `apply` for other functions like `string-append`:
  ```scheme
  (apply string-append (list "this" "and" "that")) ; produces "thisandthat"
  ```

### **Dealing with Complex Data**:
Sometimes transformations involve more complex collections like images. Consider transforming a list of numbers into a series of green circles:
```scheme
(define green-circle
  (lambda (radius)
    (circle radius "solid" "green")))
(map green-circle (list 20 40 60 40 20))
```
This produces a list of circles with different radii, which you can then combine using functions like `beside` or `above`.

### **Error Handling in `map` and `apply`**:
- If you use incorrect types, both `map` and `apply` will generate clear error messages. For example, trying to use `+` with a list of strings will raise an error.


### **Summary**:
List transformations are a powerful tool in functional programming. The **`map`** function is central to transforming individual elements of a list based on a defined function. Additionally, **`apply`** allows you to apply a function to an entire list at once. These transformations are crucial for efficiently manipulating collections of data.
