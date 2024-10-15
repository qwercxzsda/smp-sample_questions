# Midterm 2014 Spring

## Problem 2 (18 pts)

### 2.1. (2 pts)

Select all valid variable names in Python.

1. `cs101`
2. `4option`
3. `A4`
4. `IF`
5. `_2dNum`

### 2.5. (2 pts)

Write the result of the following program.

```python
y = 1
for x in range(10, 0, -3):
    y *= x
print(x, y)
```

### 2.6. (2 pts)

Write the result of the following program.

```python
y = 0
for x in range(0, 10, 1):
    if x % 2 == 0:
        continue
    y += x
print(x, y)
```

### 2.7. (2 pts)

Write the result of the following program.

```python
z = 0
for x in range(0, 10, 3):
    for y in range(x + 1, 10, 5):
        z += x + y
print(x, y, z)
```

## Problem 6 (5 pts)

아래 프로그램은 주사위 2개를 굴려서 나온 숫자의 합이 짝수면 사용자가 이기고, 홀수면 지는 프로그램이다. 주사위에서 나올 수 있는 숫자의 범위는 1~6이다. 프로그램이 정상 작동하도록 빈 칸을 채우시오.

```python
import random

"""blank 1"""
    return """blank 2"""

def print_result(a):
    if """blank 3""":
        print(f"The sum of the 2 dice is {a}. You lose.")
    else:
        print(f"The sum of the 2 dice is {a}. You win!")

def main():
    dice1 = rand_dice()
    dice2 = rand_dice()

    print(f"Dice 1: {dice1}, Dice 2: {dice2}")
    """blank 4"""

main()
```

## Problem 7 (7 pts)

아래 프로그램은 3자리 양의 정수를 랜덤하게 생성하려는 프로그램이다. 단, 각 자리의 숫자는 서로 중복되는 경우가 없다는 조건을 만족시켜야 한다. 빈 칸을 채우시오.

```python
import random

def is_duplicate(n):
    check = False

    n1 = """blank 1"""
    n10 = """blank 2"""
    n100 = """blank 3"""

    if """blank 4""":
        check = True

    return """blank 5"""

def main():
    num = """blank 6"""
    while """blank 7""":
        num = """blank 8"""

    print(num)

main()
```

## Problem 8 (7 pts)

피보나치 수열은 아래와 같이 정의된다.

$$
\begin{align*}
    &F_0 = 0\\
    &F_1 = 1\\
    &F_n = F_{n-1} + F_{n-2} \quad \text{for } n \ge 2
\end{align*}
$$

### 8.1. (4 pts)

피보나치 수를 `fibo(n)` 이라는 함수를 사용하여 구하고자 한다. 이 함수를 <u>recursion</u> 을 이용하여 작성하시오.

```python
def fibo(n):
    if """blank 1""":
        return """blank 2"""
    else:
        return """blank 3"""

def main():
    num = 12

    print(f"First {num} Fibonacci numbers:")
    for i in range(num):
        if (i + 1) % 4:
            print(f"{fibo(i): 4d}", end=" ")
        else:
            print(f"{fibo(i): 4d}")
    print()

main()
```

### 8.2. (3 pts)

위의 작성된 프로그램을 실행하였을 때, 화면에 출력되는 결과를 쓰시오.

## Problem 9 (10 pts)

### 9.1. (5 pts)

아래 프로그램은 사용자로부터 양의 정수 1 개를 입력 받아, 숫자의 순서를 거꾸로 출력하는 프로그램이다. 프로그램이 정상 작동하도록 빈 칸을 채우시오.

```python
def reverse_int(n):
    if """blank 1""":
        print(n, end="")
    else:
        """blank 3"""
        """blank 4"""

def main():
    n = int(input())
    reverse_int(n)
    print()

main()
```

실행결과

```text
입력: 54321
출력: 12345
```

### 9.2. (5 pts)

위의 함수 `reverse_int` 함수를 while 문을 이용하여 완성하시오. (재귀 함수로 작성할 수 없음)

```python
def reverse_int(n):
    while """blank 1""":
        """blank 2"""
        """blank 3"""
```

## Problem 10 (8 pts)

다음은 주어진 배열의 순서를 뒤집는 프로그램이다. 배열의 각 원소는 처음에는 배열에서의 자신의 위치 값을 할당한다. 프로그램이 정상적으로 작동하도록 빈칸을 채우시오. 추가적인 변수는 선언할 수 없으며 ARY_SIZE 를 최소 6번 사용해야 한다.

```python
ARY_SIZE = 10

def main():
    arr = """blank 1"""

    # Initialize the array arr
    for i in range("""blank 2"""):
        """blank 3"""
        print("""blank 4""", end=" ")
    print()

    # Reverse the array arr
    for i in range("""blank 5"""):
        """blank 6"""

    # Print the reversed array arr
    for i in range("""blank 7"""):
        print("""blank 8""", end=" ")
    print()

main()
```

실행 결과

```text
0 1 2 3 4 5 6 7 8 9
9 8 7 6 5 4 3 2 1 0
```

## Problem 12 (7 pts)

아래의 프로그램은 list 의 원소 중 가장 큰 값을 찾아 그 값을 출력하는 프로그램이다. List 의 크기는 1 이상이다. 빈 칸을 채우시오. (python 내장 함수 max 사용 금지)

```python
def get_max(l):
    max_val = """blank 1"""
    for i in l:
        if """blank 2""":
            """blank 3"""
    return max_val


def main():
    arr = [0, 5, 7, 3, 2, 6, 9, 1, 4, 8]

    max_val = """blank 4"""
    print(f"MAX = {max_val}")

main()
```

실행 결과

```text
MAX = 9
```
