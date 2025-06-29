# Python Strings: Worksheet

This worksheet will guide you through the essentials of working with strings in Python. We'll start with the basics and move on to more advanced manipulation techniques.

### Section 1: The Basics of Python Strings

This section covers how to create strings and perform fundamental operations.

**1.1 Creating Strings** In Python, you can create strings using single (`'`), double (`"`), or triple (`"""` or `'''`) quotes.

**Example:**

```
my_name = "Alice"
greeting = 'Hello, world!'
multi_line_story = """This is a story
that spans across
multiple lines."""

```

**1.2 String Concatenation** You can combine strings using the `+` operator.

**Example:**

```
first_name = "John"
last_name = "Doe"
full_name = first_name + " " + last_name
print(full_name)  # Output: John Doe

```

**1.3 Finding the Length of a String** The built-in `len()` function tells you how many characters are in a string.

**Example:**

```
message = "Hello"
print(len(message)) # Output: 5

```

**1.4 Accessing Characters (Indexing)** You can access individual characters in a string using their index in square brackets `[]`. Remember, Python indexing starts at `0`.

**Example:**

```
word = "Python"
print(word[0])  # Output: P
print(word[3])  # Output: h
print(word[-1]) # Output: n (Negative indexing gets characters from the end)

```

**Exercises: Section 1**

1. Create a variable called `favorite_food` and assign your favorite food to it as a string.
2. Create two string variables, one for your city and one for your country. Concatenate them to create a new variable `location` in the format "City, Country".
3. Calculate and print the number of characters in the string "Supercalifragilisticexpialidocious".
4. Given the string `verb = "Programming"`, print the first character and the last character.

### Section 2: Manipulating Strings

Let's explore some powerful built-in methods to change and analyze strings.

**2.1 Slicing** Slicing lets you get a portion of a string (a "substring").

**Example:**

```
text = "Hello, Python!"
print(text[0:5])   # Output: Hello
print(text[7:])    # Output: Python!
print(text[:5])    # Output: Hello
print(text[::2])   # Output: Hlo yhn (gets every second character)

```

**2.2 Changing Case** You can easily convert a string to all uppercase, all lowercase, or title case.

**Example:**

```
quote = "To be or not to be."
print(quote.upper())  # Output: TO BE OR NOT TO BE.
print(quote.lower())  # Output: to be or not to be.
print(quote.title())  # Output: To Be Or Not To Be.

```

**2.3 Finding and Replacing** You can find the position of a substring or replace parts of a string.

**Example:**

```
sentence = "I like cats, and I think cats are great."
print(sentence.find("cats"))    # Output: 7 (index of the first occurrence)
print(sentence.replace("cats", "dogs")) # Output: I like dogs, and I think dogs are great.

```

**Exercises: Section 2**

1. Given `data = "abcdefg"`, use slicing to get the substring "cde".
2. Take the string `messy_string = " hELLo THERE "`. Clean it up by removing the extra spaces from both ends and converting it to just have the first letter capitalized. (Hint: you might need to chain methods like `.strip()`and `.capitalize()()`).
3. Create a sentence and then replace a word in it with a different word of your choice.

### Section 3: Stretch Activities

These exercises are more challenging and may require combining several concepts.

**Activity 1: The Formatter**

Write a program that takes a user's first name and last name. Then, print a formatted welcome message that says "Welcome, [First Name] [Last Name]!", where their names are properly capitalized regardless of how they typed them.

**Example Input:** `aLIce`, `sMITh` **Example Output:** `Welcome, Alice Smith!`

**Activity 2: The Palindrome Checker**

A palindrome is a word or phrase that reads the same backward as forward (e.g., "madam", "racecar"). Write a program that checks if a given string is a palindrome. The check should be case-insensitive.

**Example Input:** `Level` **Example Output:** `Yes, it is a palindrome.`

**Example Input:** `Hello` **Example Output:** `No, it is not a palindrome.`

**(Hint:** Slicing can reverse a string very easily! `a_string[::-1]` will give you a reversed copy of `a_string`.)

**Activity 3: The Word Counter**

Write a program that counts how many words are in the following sentence.

```
the_sentence = "Python is a versatile language and it is great for beginners and experts alike."

```

**(Hint:** The `.split()` method will be very helpful here. It splits a string into a list of words.)
