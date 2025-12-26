## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
num = int(input("Enter a number: "))
temp = num
rev = 0
while temp > 0:
    rev = (10 * rev) + (temp % 10)  # Append the last digit of temp to rev
    temp = temp // 10  # Remove the last digit from temp
if rev == num:
    print(f"{num} is a palindrome!")
else:
    print(f"{num} is not a palindrome.")
```
## Output
<img width="1020" height="489" alt="image" src="https://github.com/user-attachments/assets/bf650cb8-7ab4-4834-a70d-5ecbb88782c2" />
<img width="734" height="224" alt="image" src="https://github.com/user-attachments/assets/c6322b8c-ba34-48d6-b706-819f8b93ad8d" />

## Result
Hence the program is written and executed successfully
