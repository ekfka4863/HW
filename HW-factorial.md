# HW - Factorial
<br><br>
### This is actually an assignment from last week... 
### But anyway, today I'm going to talk about 3 ways how to handle factorial! 
<br>
So as I said, we do have 3 methods ... 

>> 1. Using for-statement 

>> 2. Using recursive function

>> 3. Using math library

---
<br>

## Solution 1: For Statement
```
a = int(input("팩토리얼을 구할 숫자를 입력하세요 : ")) 
result = 1 
for item in range(1, a+1, 1): 
    result *= item                    #result = result * item 
print(result)
```
---
## Solution 2: Recursive Function
```
def my_factorial(n): 
    if(n > 1): 
        return n * my_factorial(n - 1) 
    else: 
        return 1 

a = int(input("팩토리얼을 구할 숫자를 입력하세요 : ")) 
print(my_factorial(a))
```
---
## Solution 3: Math Library
```
import math 
a = int(input("팩토리얼을 구할 숫자를 입력하세요 : ")) 
print(math.factorial(a))
```