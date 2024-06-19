[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15262039&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   - Python is a high-level, interpreted programming language known for its simplicity and readability, which makes it accessible to both beginners and experienced developers.
   - Python is easy to read,write and it is interpreted language.
   - The language is dynamically typed and support multiple pradigms.
   - Python can be used for web development, data science and Machine learning.
   - Its can also be used for Software Development and Game development.


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   Windows:
   - Download Python installer from [python](https://www.python.org/downloads/)
   - Run the installer and select "Add Python to PATH" during installation.
   - Click "Install Now" and Python will be installed.

   macOS:
   - Install Homebrew if not already installed: /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   - Install Python using Homebrew: brew install python.

   Linux(Ubuntu/Debian):
   - Open terminal and update package list: sudo apt update.
   - Install Python: sudo apt install python3.

   Verifying Installations:
   - Open terminal or command prompt.
   - Type python --version or python3 --version.
   - Verify the Python version displayed matches the installed version.

   Setting Up a Virtual Environment
   Using venv which is built in module in Python 3
   - Open terminal or command prompt.
   - Create a new directory for your project: mkdir myproject && cd myproject.
   - Create a virtual environment in windows use the command python -m venv env.
   - In macOs/Linux a command python3 -m venv env..


3. Python Syntax and Semantics:
Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

- print("Hello, World!")
- The print() function in Python is used to output data to the console. Here, it prints the string "Hello, World!"
- In Python, strings are sequences of characters enclosed in either single ' or double " quotes. They represent textual data and can include letters, numbers, and special characters.

4. Data Types and Variables:
List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   - Python Supports several basic data types which include:
   - Integer (int): Whole numbers without any decimal point.
   - Float (float): Numbers that have a decimal point or use scientific notation.
   - String (str): Ordered sequence of characters enclosed in single or double quotes.
   - Boolean (bool): Represents truth values True or False.
   - NoneType (None): Represents the absence of a value or a null value.

**Example Code Snippet:**
<pre>
   '''
         # Integer variable
             num1 = 42

         # Float variable
             num2 = 3.14
         # String variable
              message = "Hello, Python!"

         # Boolean variables
             is_python_fun = True
            is_learning = False

         # NoneType variable
           nothing_here = None

         # Printing variables and their types
            print(f"num1: {num1}, type: {type(num1)}")
            print(f"num2: {num2}, type: {type(num2)}")
            print(f"message: {message}, type: {type(message)}")
            print(f"is_python_fun: {is_python_fun}, type: {type(is_python_fun)}")
            print(f"is_learning: {is_learning}, type: {type(is_learning)}")
            print(f"nothing_here: {nothing_here}, type: {type(nothing_here)}")
   
   '''
</pre>



5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and `for` loop.
   - Conditional statements allow you to execute code based on certain conditions. The primary conditional statement in Python is the if-else statement.
   - Loops allow you to execute a block of code multiple times. The most common types of loops in Python are for loops and while loops.

**Example Code Snippet:**
<prev>
            '''
            #Conditionals
                if condition:
                # Code to execute if condition is True
            else:
                # Code to execute if condition is False

            Example of Conditionals
            number = 10

            if number > 0:
                print("Positive number")
            else:
                print("Non-positive number")


            #Example of for Loop
            for variable in sequence:
                # Code to execute for each item in the sequence

                #Example
                fruits = ["apple", "banana", "cherry"]

            for fruit in fruits:
                print(f"I like {fruit}")
            '''
</prev>

6. Functions in Python:
 What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

  - Functions in Python are blocks of organized, reusable code designed to perform a specific task. They allow you to break down your program into smaller, manageable parts, making your code more modular, readable, and easier to maintain
  - 

7. Lists and Dictionaries:
Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   - Lists are ordered collections of items accessed by index, ideal for sequences where the order matters.
   - Dictionaries are unordered collections of key-value pairs, accessed by keys, suitable for mapping relationships between data.


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   - Exception handling in Python is the mechanism that allows you to handle and respond to errors or exceptional situations that occur during the execution of a program. Exceptions are errors that disrupt the normal flow of the program, and handling them gracefully can prevent crashes and improve program robustness.

**Example Code Snippet:**
<prev>
 '''
        try:
                # Code that might raise an exception
            x = int(input("Enter a number: "))
            y = 10 / x

        except ZeroDivisionError:
                # Handle specific exception (division by zero)
            print("Error: Cannot divide by zero!")

        except ValueError:
            # Handle specific exception (invalid conversion to int)
            print("Error: Invalid input! Please enter a valid number.")

        except Exception as e:
            # Catch-all for any other exceptions
            print(f"An error occurred: {e}")

        else:
            # Executed if no exception occurs
            print(f"The result is: {y}")

        finally:
            # Optional cleanup code executed regardless of exceptions
            print("Execution complete.")
 '''
</prev>


9. Modules and Packages:
Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   - Modules in Python are files containing Python definitions (functions, classes, variables) and statements.
   -  Packages are a way of structuring Python's module namespace by using "dotted module names". A package is a directory containing Python modules and an __init__.py file to indicate that the directory should be treated as a package.


**Example Code Snippet:**
<prev>
        # Importing the math module
         import math

         # Using functions from the math module
         print(math.sqrt(16))   # Output: 4.0 (square root)
         print(math.pow(2, 3))  # Output: 8.0 (2 raised to the power of 3)
         print(math.pi)         # Output: 3.141592653589793 (value of pi)
</prev>

10. File I/O:
 How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
- To read from a file in Python, you typically follow these steps:
- Open the File: Use the open() function to open the file in read mode ('r').
- Read the File Content: Use methods like read(), readline(), or readlines() to read the content.
- Close the File: Always close the file using the close() method to free up system resources

**Example Code Snippet:**
<prev>
    ''' python
         # Example script to read and print the content of a file

        # Open the file in read mode
       file_path = 'sample.txt'  # Replace with your file path
      try:
       with open(file_path, 'r') as file:
        content = file.read()
        print(content)
        except FileNotFoundError:
        print(f"Error: File '{file_path}' not found.")
      except IOError:
         print(f"Error: Unable to read from file '{file_path}'.")
    '''
</prev>

To write to a file in Python, follow these steps:
- Open the File: Use the open() function with the appropriate mode ('w' for writing, 'a' for appending, etc.).
- Write to the File: Use the write() method of the file object to write data to the file.
- Close the File: Always close the file to save changes and free up resources.

- **Example Code Snippet:**
<prev>
```python
        # Step 1: Open the file (create it if it doesn't exist)
         with open('output.txt', 'w') as file:
            # Step 2: Write to the file
            file.write('Hello, this is a sample text!\n')
            file.write('Writing to files in Python is simple.\n')
            # Step 3: File automatically closed when exiting the 'with' block
</prev>


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


