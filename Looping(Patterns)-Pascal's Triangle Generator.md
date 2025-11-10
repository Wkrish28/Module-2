# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
Developed by: Shrikrishna V
Register.no:212223040198

rows = int(input())
coef = 1
for i in range (1, rows+1):
    for space in range (1, rows-i+1):
        print(" ",end="")
    for j in range(0, i):
        if j==0 or i==0:
            coef = 1
        else:
            coef = coef * (i - j)//j
        print(coef, end= " ")
    print()
```
## Sample Output
<img width="839" height="583" alt="image" src="https://github.com/user-attachments/assets/0370f6d5-41e1-47bb-9dff-7bd46913ca4c" />

## Result
Thus the program that generates Pascal's Triangle using numbers. The number of rows is accepted from the user has been executed successfully.
