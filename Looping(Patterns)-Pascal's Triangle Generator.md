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
n = int(input("Enter number of rows: "))
for i in range(n):
    for space in range(n - i - 1):
        print(" ", end="")

    value = 1
    for k in range(i + 1):
        print(value, end=" ")
        value = value * (i - k) // (k + 1)
    print()
```

## Sample Output
<img width="867" height="389" alt="image" src="https://github.com/user-attachments/assets/795172a4-b64b-4665-862e-db9e81c0f538" />
<img width="696" height="234" alt="image" src="https://github.com/user-attachments/assets/c5f2d36d-2b26-475c-bc54-9ccca1612564" />


## Result
Hence the program is written and executed successfully
