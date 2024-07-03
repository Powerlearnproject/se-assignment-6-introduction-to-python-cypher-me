[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15366653&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
      - Python is a high-level, interpreted programming language known for its simplicity, readability, and versatility.
      - Some key feature include: it has a simple syntax, versitile, extensive standard library, interpretaded and interactive and it is scalable
      - python can be used in web development, Data analysis, machine learning, game development and in education and training

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
      - To install python in linux you have to first check if Python is already installed on your system by opening a terminal and typing python --version or python3 --version. 
      - Update your package lists to ensure you get the latest versions of packages. 
      `sudo dnf update -y`
      - Install python through the following command `sudo dnf install python3 python3-pip`
      - verify installation through `python3 --version`

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
      ```py
      print("Hello, World!")
      ```
      -  `print` is a built-in Python function used to output or display data to the console.
      - "Hello, World!": This is a string literal, enclosed in double quotes
      - The parentheses `()` are used to enclose the arguments passed to the print function.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
      - Integers are whole numbers without a fractional part. They can be positive or negative.
      - Floats are numbers with a decimal point. They can represent fractional values.
      - Strings are sequences of characters enclosed in single, double, or triple quotes.
      - Booleans represent one of two values: `True` or `False`.
      - Lists are ordered collections of items, which can be of any data type. Lists are mutable, meaning their contents can be changed.
      - Tuples are ordered collections of items, similar to lists, but they are immutable, meaning their contents cannot be changed after creation.
      - Dictionaries are collections of key-value pairs. Each key is unique and is used to access the corresponding value. Dictionaries are mutable.
      - Sets are unordered collections of unique items. Sets are mutable.

      ```py
         # Integer variable
      age = 30

      # Floating point variable
      pi = 3.14

      # String variable
      name = "Alice"

      # Boolean variables
      is_student = True
      is_employee = False

      # List variable
      numbers = [1, 2, 3, 4, 5]

      # Tuple variable
      coordinates = (10.0, 20.0)

      # Dictionary variable
      person = {'name': 'Bob', 'age': 25, 'city': 'New York'}

      # Set variable
      unique_numbers = {1, 2, 3, 4, 5}

      # Printing variables to demonstrate their values
      print(f"Name: {name}")
      print(f"Age: {age}")
      print(f"PI value: {pi}")
      print(f"Is student: {is_student}")
      print(f"Is employee: {is_employee}")
      print(f"Numbers list: {numbers}")
      print(f"Coordinates tuple: {coordinates}")
      print(f"Person dictionary: {person}")
      print(f"Unique numbers set: {unique_numbers}")
      ```

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
      - Conditional statements and loops are fundamental control structures in Python that enable developers to control the flow of execution based on conditions and repeat tasks iteratively.

      ```py
      # if loop
         age = 30
         if age >= 18:
            print("You are an adult.")
      # else loop
         score = 75
         if score >= 60:
            print("You passed the exam.")
         else:
            print("You failed the exam.")

      # for loop
      numbers = [1, 2, 3, 4, 5]
      for number in numbers:
         print(number)

      ```

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

      - Functions in Python are blocks of reusable code that perform a specific task. They are defined using the `def` keyword, followed by the function name and parentheses containing any parameters. 
      - functions are usefull because the enable code reusability madularity, abstraction and testing.
      ```py
      def sum(a, b):
         return a + b

      sum_out = sum(3,5)
      print(sum_out)
      ```

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
      - Lists are ordered collections where elements are stored in a sequence and accessed by their index while  Dictionaries are unordered collections of key-value pairs. They do not preserve the order of insertion.
      - Elements in a list are accessed using integer indices starting from 0, Elements in a dictionary are accessed using keys rather than indices.
      - Lists can contain duplicate elements, Keys in dictionaries must be unique.
      - Lists are suitable for storing collections of items where the order matters, such as maintaining a sequence of tasks, Dictionaries are ideal for scenarios where fast lookup and mapping of unique keys to values are essential.

      ```py
      # Create a list of numbers
      numbers = [1, 2, 3, 4, 5]

      # Create a dictionary with some key-value pairs
      person = {
         'name': 'Alice',
         'age': 30,
         'city': 'New York'
      }

      # Demonstrate basic operations on the list
      print("Original list of numbers:", numbers)

      # Append a number to the list
      numbers.append(6)
      print("After appending 6:", numbers)

      # Remove a number from the list
      numbers.remove(3)
      print("After removing 3:", numbers)

      # Access an element by index
      print("Element at index 2:", numbers[2])

      # Modify an element by index
      numbers[1] = 20
      print("After modifying element at index 1:", numbers)

      # Demonstrate basic operations on the dictionary
      print("\nOriginal dictionary:", person)

      # Add a new key-value pair
      person['email'] = 'alice@example.com'
      print("After adding email:", person)

      # Remove a key-value pair
      del person['city']
      print("After removing city:", person)

      # Access a value by key
      print("Name:", person['name'])

      # Modify a value by key
      person['age'] = 31
      print("After modifying age:", person)

      # Check if a key exists in the dictionary
      if 'email' in person:
         print("Email exists in the dictionary")

      # Iterate over the dictionary keys and values
      print("\nDictionary items:")
      for key, value in person.items():
         print(f"{key}: {value}")
      ```

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
      - Exception handling in Python refers to the process of anticipating and handling runtime errors (exceptions) that may occur during program execution. When an error occurs in Python, it raises an exception, which interrupts the normal flow of the program.
      ```py
      def divide_numbers(a, b):
         try:
            result = a / b  # Attempt division
            print(f"Result of division: {result}")

         except ZeroDivisionError as e:
            # Handle division by zero error
            print(f"Error: {e}")

         finally:
            print("Division operation completed.")

      # Test cases
      divide_numbers(10, 2)   # Normal division
      divide_numbers(5, 0)    # Division by zero error
      ```

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
      - In Python, modules and packages are organizational units used to structure and manage code effectively, promote code reusability, and facilitate modular programming practices.
      ```py
      import math

      number = 25
      square_root = math.sqrt(number)
      print(f"Square root of {number} is: {square_root}")
      ```

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
      - In Python, reading from and writing to files is straightforward using built-in functions and methods provided by the language.
      ```py

      file_path_read = 'file1.txt'
      file_path_write = 'file2.txt' 
      try:

         with open(file_path_read, 'r') as file:

            content = file.read()
            print(f"Content of '{file_path_read}':")
            print(content)

      except FileNotFoundError:
         print(f"Error: File '{file_path_read}' not found.")

      except IOError as e:
         print(f"Error reading file: {e}")


      lines_to_write = [
         "Line 1: Hello, World!",
         "Line 2: This is a test.",
         "Line 3: Writing to a file in Python."
      ]

      try:

         with open(file_path_write, 'w') as file:

            for line in lines_to_write:
                  file.write(line + '\n')
         
         print(f"Successfully wrote {len(lines_to_write)} lines to '{file_path_write}'.")

      except IOError as e:
         print(f"Error writing to file: {e}")
      ```


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].



