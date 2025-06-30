## Part 2: Python Dictionaries

### 🧊 Easy Questions

**1. Create a Dictionary:** Create a dictionary named `person` that stores the following information: `name` is "John Doe", `age` is 30, and `city` is "New York". Print the dictionary.

**2. Access a Value:** Using the `person` dictionary from the previous question, access and print the value associated with the key "age".

**3. Add a Key-Value Pair:** Add a new key-value pair to the `person` dictionary: "occupation" with the value "Engineer". Print the updated dictionary.

**4. Update a Value:** Update the `city` in the `person` dictionary to "San Francisco". Print the updated dictionary.

### 🔥 Medium Questions

**1. Iterate and Print Keys:** Given the dictionary `capitals = {"USA": "Washington D.C.", "France": "Paris", "Japan": "Tokyo"}`, write a loop to print all its keys.

**2. Iterate and Print Values:** Using the `capitals` dictionary, write a loop to print all its values.

**3. Iterate and Print Items:** Using the `capitals` dictionary, write a loop to print each key-value pair in the format: "The capital of [Country] is [Capital]".

**4. Check if a Key Exists:** Write code to check if the key "Germany" exists in the `capitals` dictionary. If it doesn't, add it with the value "Berlin". Print the final dictionary.

**5. Merging Dictionaries:** You have two dictionaries: `dict1 = {'a': 1, 'b': 2}` `dict2 = {'b': 3, 'c': 4}`Merge `dict2` into `dict1`. If there are overlapping keys, the values from `dict2` should overwrite the values from `dict1`. Print the merged dictionary.

### 🌶️ Hard Questions

**1. Nested Dictionary Access:** You are given a nested dictionary representing a student's grades: `student = { "name": "Alice", "grades": { "math": 92, "science": 88, "history": 95 } }` Write code to access and print Alice's science grade.

**2. Invert a Dictionary:** Given a dictionary `data = {"A": 1, "B": 2, "C": 3}`, create a new dictionary where keys and values are swapped. Assume all values are unique. The result should be `{1: "A", 2: "B", 3: "C"}`. Print the new dictionary.

**3. Word Frequency Counter:** Write a function that takes a string of text and returns a dictionary where the keys are the words in the text and the values are the number of times each word appeared. The function should be case-insensitive. Example input: `"The quick brown fox jumps over the lazy dog"` Example output: `{'the': 2, 'quick': 1, 'brown': 1, 'fox': 1, 'jumps': 1, 'over': 1, 'lazy': 1, 'dog': 1}`