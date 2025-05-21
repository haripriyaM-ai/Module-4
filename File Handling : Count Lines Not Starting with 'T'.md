# EXP 20: File Handling in Python: Count Lines Not Starting with 'T'

##  Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

##  Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

##  Program
```
file_path = "story.txt"
with open(file_path, "w") as file:
    file.write("This is a sample line.\nThat begins with T.\nAnother line.\nYet another.\nTea time.\nCoding begins.\n")

count = 0
with open(file_path, "r") as file:
    for line in file:
        if not line.startswith("T"):
            count += 1

print(count)
```

## Output
![image](https://github.com/user-attachments/assets/c3032f59-5ceb-49b4-9d61-433c12e8457c)

## Result
Thus, the program is verified successfully.
