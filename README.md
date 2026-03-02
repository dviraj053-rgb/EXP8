# EXP8
Here is the **rephrased version** of your experiment in a clear and structured format:

---

# **Aim: Study of For Loop in Python**

---

## **Theory**

The `for` loop in Python is used to iterate over a sequence (or iterable). Its basic syntax is:

```
for item in iterable:
```

When this statement executes, Python internally checks whether the object being looped over is an **iterable**. An iterable is any object that can return its elements one at a time. Python creates an **iterator** from the iterable, which keeps track of the current position and provides the next value until all elements are exhausted.

---

## **Key Components of a For Loop**

### **1. Target Variable**

The target variable (e.g., `item`) acts as a placeholder. During each iteration, it is automatically assigned the next value from the iterable.

### **2. The Iterable**

An iterable is any object capable of returning its elements one by one. Examples include:

* **Sequences:** Lists, Tuples, Strings, Ranges
* **Mappings:** Dictionaries (iterate over keys by default)
* **Collections:** Sets

---

## **The `range()` Function**

Since Python loops operate over iterables, the `range()` function is commonly used when we want to repeat an action a fixed number of times.

Technically, `range()` is an immutable sequence type, not just a regular function. When `range(5)` is used, Python does not store all numbers in memory. Instead, it creates a **range object** that generates numbers as needed (lazy evaluation). This makes it highly memory-efficient.

### **Syntax: `range(start, stop, step)`**

* **Start:** Starting value (inclusive). Default is 0.
* **Stop:** Ending value (exclusive).
* **Step:** Interval between numbers (can be positive or negative).

---

## **Control Flow Statements**

To control the execution of loops, Python provides:

* **break:** Immediately stops the loop.
* **continue:** Skips the remaining code in the current iteration and moves to the next one.
* **else:** Executes only if the loop completes normally (without encountering `break`).

---

## **Nested Loops**

Python allows loops inside other loops. In nested loops, the inner loop runs completely for every single iteration of the outer loop. Nested loops are commonly used in matrix operations and pattern printing.

---

## **Example: Multiplication of Two 3×3 Matrices**

```
for i in range(3):      # Rows of matrix A
    for j in range(3):  # Columns of matrix B
        for k in range(3):
            result[i][j] += a[i][k] * b[k][j]

for row in result:
    print(row)
```

---

# **Algorithms**

---

## **A) Print Even Numbers from 1 to 10**

Start
Initialize loop from i = 2 to 10 with step 2
Print i in each iteration
End

---

## **B) Sum of First n Numbers**

Start
Input integer n
Initialize sum = 0
Loop from i = 1 to n
Add i to sum
After loop, print sum
End

---

## **C) Print a 3×3 Matrix**

Start
Define a 3×3 matrix
Outer loop: iterate rows (i = 0 to 2)
Inner loop: iterate columns (j = 0 to 2)
Print element a[i][j] with space
After each row, print newline
End

---

## **D) Matrix Multiplication (3×3)**

Start
Define matrices a and b
Initialize result matrix with zeros
Outer loop: iterate rows of a
Middle loop: iterate columns of b
Inner loop: calculate dot product
Update result[i][j]
After loops, print result matrix
End

---

## **E) Combinations of Three Unequal Numbers**

Start
Define list d = [1, 2, 3]
Use three nested loops (i, j, k)
Check condition:
d[i] ≠ d[j], d[j] ≠ d[k], and d[i] ≠ d[k]
If true, print combination
End

---

## **F) Pattern Printing**

### **Right-Angle Triangle**

Start
Loop i from 1 to 9
Print "* " repeated i times
End

### **Pyramid Triangle**

Start
Set rows = 5
Loop i from 1 to rows
Print spaces (rows − i)
Print "* " repeated i times
End

---

## **Conclusion**

Thus, the `for` loop was successfully studied and implemented in Python. Various programs were executed using single and nested loops. The experiment demonstrated how `for` loops efficiently handle iteration, matrix operations, combinations, and pattern printing, making programs more structured and readable.

