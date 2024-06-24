[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15321369&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

      Python is a high-level, interpreted programming language known for its readability , simplicity and  support  for multiple programming paradigms, including procedural, object-oriented, and functional programming.

      Key Features of Python:

      -Readability: Python's syntax is clear and easy to read, making it accessible to beginners.
      -Versatility: Python can be used for web development, data analysis, artificial intelligence, scientific computing, and more.
      -Large Standard Library: Python comes with a rich standard library that provides tools suited to many tasks.
      -Community Support: A large and active community means plenty of resources, libraries, and frameworks are available.
      -Cross-Platform: Python runs on various operating systems like Windows, macOS, and Linux.

      Use Cases:
      -Web Development (Django, Flask)
      -Data Science and Machine Learning (Pandas, NumPy, Scikit-Learn)
      -Automation and Scripting
      -Software Development and Prototyping
      -Game Development (Pygame)

2. Installing Python:
Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

      Installing python in kali linux
      -sudo apt install python.

      Verifying Installation
      -python --version

      Virtual Environment setup
      -python -m venv myenv
      source myenv/bin/activate

3. Python Syntax and Semantics:
Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

      print("Hello, World!")
      print: A function that outputs text to the console.
      "Hello, World!": A string literal enclosed in double quotes.

4. Data Types and Variables:
List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

      -Basic Data Types:

      int: Integer numbers (e.g., 1, 2, 3)
      float: Floating-point numbers (e.g., 1.0, 2.5)
      str: String literals (e.g., "Hello")
      bool: Boolean values (e.g., True, False)

      -Script Demonstrating Variables
      age = 25  # int
      height = 5.9  # float
      name = "Alice"  # str
      is_student = True  # bool

      print(f"Name: {name}, Age: {age}, Height: {height}, Student: {is_student}")


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

         Purpose:
      -Evaluate a condition and execute different code blocks based on whether the condition is True or False.

            Types of Conditional Statements:
      -if statement: Executes a block of code if the specified condition is True.
      -if-else statement: Executes one block of code if the condition is True and another block if it's False.
      -elif statement: Used within an if statement to check additional conditions if the initial condition is False. You can chain multiple elif statements.

      age = 18
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")


            Applications   
      -Making decisions based on user input, data values, or external factors.
      -Validating user input (e.g., ensuring age is a positive number).
      -Controlling different program functionalities based on conditions.


      Purpose:
      -Repeat a block of code a specific number of times or until a certain condition is met.

      Types of Loops:
      -for loop: Iterates through a sequence of items (like a list or string) and executes the code block for each item.
      -while loop: Continues executing the code block as long as the specified condition remains True.

      for i in range(5):
          print(i)


      Applications
      -Processing sequences of data (e.g., iterating through a list of products).
      -Performing repetitive tasks until a condition is met (e.g., guessing a number game).
      -Automating tasks that involve repetitive steps.

6. Functions in Python:
What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

  - Functions are reusable blocks of code that perform specific tasks.

  Why are Functions Useful?

      -Reusability: Once you define a function, you can call it multiple times throughout your program with different arguments if needed. This saves you from writing the same code repeatedly.
      -Modularity: Functions break down complex programs into smaller, manageable blocks of code, improving readability and organization.
      -Maintainability: If you need to modify a specific functionality, you only need to change the code within the relevant function, making updates easier.
      -Clarity: Functions with descriptive names enhance code understanding by clearly indicating what they do.

      def add(a, b):
         return a + b

      result = add(3, 4)
      print(result)  # Output: 7


7. Lists and Dictionaries:
Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

      Differences:

      Lists: Ordered collections of items, indexed by position.
      Dictionaries: Unordered collections of key-value pairs.

      # List
      numbers = [1, 2, 3, 4, 5]
      print(numbers[2])  # Accessing the third element

      # Dictionary
      person = {
         "name": "Alice",
         "age": 25,
         "city": "New York"
      }
      print(person["name"])  # Accessing value by key


8. Exception Handling:
What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

      -Exception handling in Python is a mechanism for managing errors (exceptions) that may arise during program execution.

      try:
         x = 1 / 0
      except ZeroDivisionError:
         print("Cannot divide by zero!")
      finally:
         print("Execution completed.")


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

Module: A single Python file containing definitions and statements.
Package: A collection of modules in a directory with an __init__.py file.

import math

print(math.sqrt(16))  # Output: 4.0


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

-Reading contents of a file
    with open('example.txt', 'r') as file:
    content = file.read()
    print(content)
    

--writing to a file
    lines = ["First line", "Second line", "Third line"]
   with open('output.txt', 'w') as file:
    for line in lines:
        file.write(line + "\n")


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


