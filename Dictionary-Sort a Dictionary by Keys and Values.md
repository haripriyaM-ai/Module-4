# EXP 18: Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

---

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

