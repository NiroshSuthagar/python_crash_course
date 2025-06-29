# 3 Week Python Course

# List Excercise

## Section 1: Beginner - The Basics of Python Lists

This section covers the essential operations for getting started with lists in Python.

**1.1 Creating Lists**

In Python, a list is an ordered collection of items. You can create a list by placing comma-separated values inside square brackets `[]`.

**Example:**


my_first_list = [1, 2, 3]

fruits = ["apple", "banana", "cherry"]

mixed_list = [1, "hello", 3.14]

**Exercises:**

1. Create a list named `colors` containing the strings "red", "green", and "blue".
2. Create a list named `numbers` containing the integers from 1 to 5.
3. Create an empty list named `empty_list`.

**1.2 Accessing List Elements (Indexing)**

Each item in a list has an index, which is its position in the list. Python uses zero-based indexing, meaning the first element is at index 0.

**Example:**


fruits = ["apple", "banana", "cherry"]
print(fruits[0])  # Output: apple
print(fruits[2])  # Output: cherry

You can also use negative indexing to access elements from the end of the list. `-1` refers to the last item, `-2` to the second to last, and so on.

**Example:**


fruits = ["apple", "banana", "cherry"]
print(fruits[-1]) # Output: cherry

**Exercises:**

1. Given the list `animals = ["cat", "dog", "bird", "fish"]`, what is the index of "bird"?
2. From the `animals` list, print the first element.
3. From the `animals` list, print the last element using negative indexing.

**1.3 Adding Elements to a List (`append()` and `insert()`)**

You can add new items to a list using the `append()` method, which adds an item to the end of the list.

**Example:**


fruits = ["apple", "banana"]

fruits.append("cherry")

print(fruits)  # Output: ['apple', 'banana', 'cherry']

To insert an item at a specific position, you can use the `insert()` method. It takes two arguments: the index and the value.

**Example:**


fruits = ["apple", "cherry"]

fruits.insert(1, "banana")

print(fruits)  # Output: ['apple', 'banana', 'cherry']

**Exercises:**

1. Create a list of your favorite hobbies.
2. Add a new hobby to the end of your list using `append()`.
3. Add a new hobby at the beginning of your list using `insert()`.

---

### Section 2: Intermediate - Manipulating Lists

This section introduces more advanced techniques for working with lists.

**2.1 Slicing Lists**

Slicing allows you to get a sub-list from a list. You specify a range of indices.

**Example:**


numbers = [0, 1, 2, 3, 4, 5]

print(numbers[2:5])  # Output: [2, 3, 4]

print(numbers[:3])   # Output: [0, 1, 2]

print(numbers[3:])   # Output: [3, 4, 5]

**Exercises:**

1. Given the list `letters = ['a', 'b', 'c', 'd', 'e', 'f']`, create a new list containing the elements from 'b' to 'd'.
2. From the `letters` list, create a new list containing the first three elements.
3. From the `letters` list, create a new list containing the last two elements.

**2.2 Removing Elements (`remove()`, `pop()`, and `del`)**

You can remove items from a list in several ways:

- `remove()`: Removes the *first* occurrence of a specific value.
- `pop()`: Removes the item at a given index and returns it. If no index is specified, it removes and returns the last item.
- `del`: Removes an item at a specific index.

**Example:**



fruits = ["apple", "banana", "cherry", "banana"]

fruits.remove("banana")

print(fruits)  # Output: ['apple', 'cherry', 'banana']


removed_fruit = fruits.pop(1)

print(removed_fruit) # Output: cherry

print(fruits)      # Output: ['apple', 'banana']


del fruits[0]

print(fruits)      # Output: ['banana']

**Exercises:**

1. Create a list of numbers from 1 to 5. Remove the number `3` from the list using `remove()`.
2. Create another list of numbers from 1 to 5. Remove the element at index 2 using `pop()`.
3. Create a third list of numbers from 1 to 5. Remove the first element using `del`.

**2.3 Sorting Lists (`sort()` and `sorted()`)**

You can sort the elements of a list in place using the `sort()` method.

**Example:**


numbers = [3, 1, 4, 1, 5, 9, 2, 6]

numbers.sort()

print(numbers)  # Output: [1, 1, 2, 3, 4, 5, 6, 9]


numbers.sort(reverse=True)

print(numbers)  # Output: [9, 6, 5, 4, 3, 2, 1, 1]

The `sorted()` function returns a new sorted list without modifying the original.

**Example:**



numbers = [3, 1, 4, 1, 5, 9, 2, 6]

sorted_numbers = sorted(numbers)

print(sorted_numbers) # Output: [1, 1, 2, 3, 4, 5, 6, 9]

print(numbers)      # Output: [3, 1, 4, 1, 5, 9, 2, 6]

**Exercises:**

1. Create a list of your favorite movies as strings. Sort this list alphabetically.
2. Create a list of random numbers. Create a new sorted list from it in descending order without changing the original list.

---

### Section 3: STRETCH - Complex List Operations

This section explores more powerful and efficient ways to work with lists.

**3.1 List Comprehensions**

List comprehensions provide a concise way to create lists. They consist of brackets containing an expression followed by a `for` clause.

**Example:**



# Create a list of squares from 0 to 9

squares = [x**2 for x in range(10)]

print(squares)  # Output: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]


# Create a list of even numbers from 0 to 9

evens = [x for x in range(10) if x % 2 == 0]

print(evens)    # Output: [0, 2, 4, 6, 8]

**Exercises:**

1. Use a list comprehension to create a list of the first 10 even numbers.
2. Use a list comprehension to create a list of the lengths of the words in the following sentence: "the quick brown fox jumps over the lazy dog".
3. Given a list `numbers = [1, 2, 3, 4, 5, 6]`, use a list comprehension to create a new list containing only the numbers that are divisible by 3.

**3.2 Nested Lists**

A nested list is a list that contains other lists.

**Example:**



matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

print(matrix[1][1]) # Output: 5

**Exercises:**

1. Create a 3x3 nested list representing a Tic-Tac-Toe board, with all elements initially being an empty string `""`.
2. Access and print the element in the second row and third column of your Tic-Tac-Toe board.
3. Using nested loops, iterate through the `matrix` from the example and print each element on a new line.

**3.3 Lists with Loops and Conditionals**

Combining lists with loops and conditional statements allows for powerful data processing.

**Example:**


numbers = [1, 15, -7, 8, 23, -4]

positive_numbers = []

for num in numbers:
    if num > 0:
        positive_numbers.append(num)
        
print(positive_numbers) # Output: [1, 15, 8, 23]

**Exercises:**

1. Given a list of numbers, write a program that finds the largest and smallest numbers in the list.
2. You are given a list of strings. Write a program that creates a new list containing only the strings that have a length greater than 5.
3. Write a program that takes two lists and returns a new list containing only the elements that are common to both lists.

---
