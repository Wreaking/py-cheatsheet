# py-cheatsheet
the full explanation of python
# Introduction 
Hello there, im Abdul Qaadir Mohiuddin Riaz aka Wreaking own this repo and this repo can only accessed by my fellow hackathon team., This repo is based upon the complete course of python. 
- I made these notes, because I usually forget some stuff about Python. So I used to refer from these notes.
- I thought of sharing these notes with everyone, because everyone deservers to learn Python.
- I tried my best to make it easy for you guys, so that you understand the basic concept.
- You need to practice it on a daily basis, if you are willing to learn Python.
So let's begin!
```py
print("Hello World")
```
## Chapter1: Errors
Mistakes made ina program are called errors and there are two main types of errors:
## Syntax error
It occurs when you write some code that isn't allowed in the python language. For example if we type this code line:
```py
print("Hello world)
```
![image](https://github.com/user-attachments/assets/49b01b64-8f1d-4252-a49a-a558e98aeb08)
> Why is that? Python wont able to tell where the string of the text[will be discussed later] ends.
> Therefore we write,
```py
print("hello world")
# output: Hello World
```
## Run-time errors
Some IDLE(visual studio code, pycharm etc) catches syntax errors before running/executing the program or code but some errors cannot be caught until the program is executed. These errors are known as run-time errors because it only occurs at the time when the program is executed. For example:
```py
print(hello world)
```
![image](https://github.com/user-attachments/assets/c34f27f5-6281-407c-b52a-4aa8e24f4922)
This error is occurred because the python thinks "hello" is a variable[will be discussed later] and that variable is not defined.
### Common Types of Run-Time Errors
- ZeroDivisionError: Trying to divide a number by zero.
```py
result = 10 / 0  # This will cause an error
```
![image](https://github.com/user-attachments/assets/1454a991-1f39-4e4a-afa4-72c4393fffc5)
- IndexError: Trying to access a list item that doesn’t exist.
```py
my_list = [1, 2, 3]
print(my_list[3])  # Index 3 is out of range
```
![image](https://github.com/user-attachments/assets/eb0a1c95-1139-44e8-afa1-0e2f15b23dc6)
- TypeError: Mixing up data types, like adding a number to a string.
```py
result = 'Hello' + 5  # Cannot combine a string and a number
```
![image](https://github.com/user-attachments/assets/190ccb57-f794-4c4c-b9d1-effcb0d11c14)
## Logical Errors
Logical errors occur when your code runs without any crashes or error messages, but it produces the wrong results. This means the code is written correctly in terms of syntax (grammar) but does not do what you want it to do. For example
```py
def add_numbers(a, b):
    return a - b  # Mistake: This should be addition, not subtraction
result = add_numbers(2, 3)  # You expect 5, but it will return -1
```
> This is a function[will be discuused later] where we are trying to add two numbers but instead of adding, you are subracting. This is a human phenomenon! These errors usually happen because of a mistake in your logic or reasoning. You might have meant to do one thing, but you wrote the code to do something different.
### AttributeError
This happens when you try to access something that doesn’t exist on an object, like a method or property or AttributeError occurs in Python when you try to access an attribute or method (a function that belongs to an object) that doesn’t exist for that particular object.
```py
my_string = "Hello"
my_string.append(" World")  # This will cause an AttributeError
```
![image](https://github.com/user-attachments/assets/64da76d4-3779-4750-afdb-a69bbed7e77a)
Correct way is:
```py
my_string = ["Hello"] # known as List
my_string.append(" World")  # Strings don’t have an append method
print(my_string) # output will be ["Hello", " World"]
```
## ValueError
This happens when a function gets the right type of argument but the value is inappropriate.
```py
a = int("abc")  # Cannot convert 'abc' to an integer
a = "hello there"
print(a)
```
![image](https://github.com/user-attachments/assets/ad0f9bc8-9537-4ab0-a0f8-482f1e9d3271)
> Correct way is
``` py
a = int(1)  # Cannot convert 'abc' to an integer
print(a) # Ouput will be 1
```
## KeyError
This occurs when you try to access a key in a dictionary that doesn’t exist.
```py
my_dict = {
           'a': 1
          }
print(my_dict['b'])  # 'b' key does not exist
```
![image](https://github.com/user-attachments/assets/a9a10142-88fb-4fad-a3e7-d03afacce96f)
Correct way is:
```py
my_dict = {
    'a': 1,
    'b': 2
    }
print(my_dict['b']) #output will be 2
```
## IndentationError
 An IndentationError occurs in Python when the code is not properly indented. Python uses indentation (spaces or tabs) to define the structure of the code, such as which lines belong to a function, loop, or condition.

```py
def my_function():
print("Hello")  # Incorrect indentation
```

Correct way is:
```py
def my_function():
    print("Hello World") #output will be Hello World
# ^^ this space is known as indentation
```
# PEP 8
PEP 8, or Python Enhancement Proposal 8, is the style guide for Python code. It provides conventions and best practices to improve the readability and consistency of Python code. Some key points include:

1. **Indentation**: Use 4 spaces per indentation level.
2. **Line Length**: Limit lines to 79 characters.
3. **Blank Lines**: Use blank lines to separate functions and classes, and larger blocks of code inside functions.
4. **Imports**: Import modules at the top of the file and group them logically (standard libraries, third-party libraries, local applications).
5. **Naming Conventions**: Use lowercase with underscores for functions and variable names, and CamelCase for class names.
6. **Comments**: Write comments to explain code, and use inline comments sparingly. Docstrings should describe modules, classes, and functions.
7. **Whitespace**: Avoid excessive whitespace in expressions and statements.

Following PEP 8 helps make Python code more understandable and maintainable, especially when working in teams. You can find the full PEP 8 document on the official Python website for a comprehensive guide.

[Click me](https://github.com/Wreaking/py-cheatsheet/blob/Chapter2-Variables/README.md) for the next topic!
