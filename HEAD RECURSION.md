# 🔁 Types of Recursion: Head Recursion in Python

## 🎯 AIM:
To write a Python program to demonstrate **Head Recursion** by finding and printing the sequence based on the sum of all digits (even or odd adjusted input).

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `fun(n)`
3. In the function:
   - Create a recursive call at the **beginning** (Head Recursion)
   - Print the result after the recursive call
4. Take input from the user
5. If input is odd, convert it to the next even number
6. Call the recursive function
7. **Stop**

## 💻 PROGRAM:
```
def sum_digits(n):
    return sum(int(d) for d in str(n))

def fun(n):
    if n <= 0:
        return
    fun(n - 2)  # Head recursion
    print(f"{n} → {sum_digits(n)}")

num = int(input("Enter a number: "))
if num % 2 != 0:
    num += 1
fun(num)
```

## OUTPUT
![446524897-4ef27fe9-79cc-4185-b784-857e3fc4d71a](https://github.com/user-attachments/assets/d46234b6-0032-450e-bddd-c8d83f82ec2a)



## RESULT
Thus, the program executed successfully
