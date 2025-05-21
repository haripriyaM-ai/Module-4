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
