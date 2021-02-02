# HackerRank - List Comprehensions
<br>

> ## List Comprehension VS For Loop in Python

- Problem:
```
You are given three integers x, y and z representing the dimensions of a cuboid along with an integer n. Print a list of all possible coordinates given by (i, j, k) on a 3D grid where the sum of i + j +k is not equal to n. 
Here, 0<=i<=x; 0<=j<=y; 0<=k<=z. Please use list comprehensions rather than multiple loops, as a learning exercise.
```

- Example:
<img src="././HackerRank-List_Comprehension.png">
<br>
<hr>

> ## Solution 1: Multiple Loop
<br>

```
answer_list = []

for a in range(x+1):
    for b in range(y+1):
        for c in range(z+1):
            if a + b + c != n:
                (answer_list).append([a, b, c])

print(answer_list)
```
<hr>

> ## Solution 2: List Comprehension
<br>

```
if __name__ == '__main__':
    x = int(input())
    y = int(input())
    z = int(input())
    n = int(input())

answer_list = []

answer_list = ([[a,b,c] for a in range(x+1) for b in range(y+1) for c in range(z+1) if (a + b + c) != n])

print(answer_list)
```
<hr>

- cf .
    - https://www.programiz.com/python-programming/list-comprehension



