# Midterm 2010 Spring

## Problem 2 (4 pts)

### 2.1. (2 pts)

The following program generates a random integer in the range 1 to 6. To complete the program, fill out the blanks.

```python
import random

def main():
    x = """blank"""
    print(x)

main()
```

### 2.2. (2 pts)

The following program generates a random real numbers in the range 1 to 2. To complete the program, fill out the blanks.

```python
import random

def main():
    x = """blank"""
    print(x)

main()
```

## Problem 3 (10 pts)

Write a program that splits one-, ten-, and hundred-digit for a given number n. We assume the number is between 0 and 999.
For example, the output of the following program should be

```text
123 = 3*1 + 2*10 + 1*100
123 = 3*1 + 2*10 + 1*100
```

```python
def main():
    n = 123

    one, ten, hundred = split(n)
    print(f"{n} = {one}*1 + {ten}*10 + {hundred}*100")
    print(f"{n} = {split_one(n)}*1 + {split_ten(n)}*10 + {split_hundred(n)}*100")

main()
```

In other words, write the source code for the following user-defined functions `split_one`, `split_ten`, `split_hundred`, and `split`.

```python
def split_one(n):
    """blank"""
```

```python
def split_ten(n):
    """blank"""
```

```python
def split_hundred(n):
    """blank"""
```

```python
def split(n):
    """blank"""
```

## Problem 4 (12 pts)

This is a program which prints four right triangles below.

```text
    * *
   ** **
  *** ***
 **** ****
***** *****

***** *****
 **** ****
  *** ***
   ** **
    * *
```

To complete the program, fill out the blanks.

```python
def main():
    for i in range(11):
        if i < 5:
            for j in range(5):
                if """blank 1""":
                    print("*", end="")
                else:
                    print(" ", end="")
            print(" ", end="")
            for j in range(5):
                if """blank 2""":
                    print("*", end="")
                else:
                    print(" ", end="")
            print()
        elif i > 5:
            for j in range(5):
                if """blank 3""":
                    print("*", end="")
                else:
                    print(" ", end="")
            print(" ", end="")
            for j in range(5):
                if """blank 4""":
                    print("*", end="")
                else:
                    print(" ", end="")
            print()
        else:
            print()

main()
```

## Problem 5 (10 pts)

This is a program using <u>recursion</u>. The program receives a positive integer as an input and converts it into the corresponding binary number. Function dec2bin must return an integer. Fill out the blanks.

Example)

```text
Input the number: 10
The decimal number 10 is represented in binary as 1010.
Input the number: 22
The decimal number 22 is represented in binary as 10110.
```

```python
def dec2bin(n):
    if """blank 1""":
        return n
    else:
        return """blank 2"""

def main():
    number = input("Input the number: ")
    result = dec2bin(int(number))

    print(f"The decimal number {number} is represented in binary as {result}.")

main()
```

## Problem 10 (9 pts)

Complete the <u>recursive</u> function `sum(n, m)`, which computes the sum of integers from n to m. For example, `sum(3, 6)` returns 18.

```python
def sum(n, m):
    if """blank 1""":
        return """blank 2"""
    else:
        return """blank 3"""
```

## Problem 11 (12 pts)

Complete the <u>recursive</u> function `seq(i)`, which computes the following sequence $a_n$ (=p) and $b_n$ (=q) and return the tuple `(p, q)`.

$$
\begin{align*}
    &a_n = 2a_{n-1} + b_{n-1}\\
    &b_n = b_{n-1} + a_{n-1}\\
    &a_1 = 2\\
    &b_1 = 1
\end{align*}
$$

For example, the main function will display the results as follows.

```text
i=1, p=2, q=1
i=2, p=5, q=3
i=3, p=13, q=8
i=4, p=34, q=21
```

```python
def seq(i):
    if i > 1:
        """blank 1"""
        return """blank 2"""
    else:
        return """blank 3"""

def main():
    for i in range(1, 5):
        p, q = seq(i)
        print(f"i={i}, p={p}, q={q}")

main()
```
