## MODULE - 4
# EXP 16: Classes and Objects in Python: Calculate the Area of a Circle

##  Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

##  Program

```
import math
class cse:
    def mech(self,radius):
        Area=math.pi*radius**2
        print(f"Area of circle: {Area:.2f}")
        
radius=float(input())
object=cse()
object.mech(radius)
```
## Output
![image](https://github.com/user-attachments/assets/d5d516ec-a77e-445c-8426-8a79984e7f29)

## Result
Thus, the program is verified successfully

---

## EXP 17: Dictionary Operations in Python: Merging Two Dictionaries

## Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## Program
```
dict1 = {'a': 1, 'b': 2}
dict2 = {'b': 3, 'c': 4}

def merge():
    merged = {**dict1, **dict2}
    print(merged)

merge()
```

## Output
![image](https://github.com/user-attachments/assets/0309f28d-5fee-4a36-8d82-6c2fac2ad17d)

## Result
Thus, the program is verified successfully.

---

# EXP 18: Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values



## Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order


## Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**


## Program
```
d = {'sherlock': 100, 'Tewksberry': 67, 'Enola': 101}

sorted_by_keys = dict(sorted(d.items()))
sorted_by_values = dict(sorted(d.items(), key=lambda item: item[1]))

print("Original:", d)
print("Sorted by keys:", sorted_by_keys)
print("Sorted by values:", sorted_by_values)
```

## Output
![image](https://github.com/user-attachments/assets/4f1fd1bf-34d4-439b-b885-712ca112374d)

## Result
Thus, the program is verified successfully.

---

# EXP 19: Exception Handling in Python: Avoiding Index Errors

##  Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## Algorithm
1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## Program
```
list1 = [20,30,40,50]
try:
    print(list1[5])
except IndexError:
    print("You're out of list range")
```

## Output
![image](https://github.com/user-attachments/assets/7e16d662-a428-467f-8d41-b12c34e2f22f)

## Result
Thus, the program is verified successfully.

---

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
