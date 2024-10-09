# Data Type: Strings
Many programmers deal with text on a daily basis for example web developers work with text that gets input from web forms. Collections of text in python are called strings. String methods are built-in functions in Python that allow you to perform various operations on strings. These methods help you manipulate, analyze, and format strings easily.
String are one of the fundamental python data type. The term data type refers to what kind of data a value represents and string is the fundamental datat type.

You can create a string by enclosing characters in 
> single quotes ('), 
> double quotes ("),
> triple quotes (''' or """).

The string data type has a special abbreviated name in python i.e `str()`. You can see by using the `type()` function which is 

Strings have three properties:
> Strings contains characters, which is individuals letters or symbols.
> Strings have lenght, which is the number of characters contained in the string.

## String Literals
You can create a string by sorrounding some text with qoutation marks:
Single(' ')
```py
str1 = 'hello world'
str2 = '12345......'
```
Double(" ")
```py
str1 = 'hello world'
str2 = '12345......'
```
Whenever you create a string by sorrounding text with qoutation marks, the string is called as string literals. The quotes sorrounding a string is known as ***delimiters***. because they tell python where a string begins and where it ends. When one type of quotes is used as a delimiter the other type of quote can be used inside of the string:
```py
str1 = "we're all"
str2 = "abid ali said, 'gullu dada ke biryani khalinge ji'"
```

If you do this:
```py
str1 = 'we'll do this'
# or
str2 = "faiz said, "i love chubby moiz"
```

Python send syntax error because it thinks that the string ends after the second " and odesnt know how to intepret the rest of the line.

## Lenght of the String
The numbers of characters contained in a string for example "abc" is a string having 3 characters/letters. Therefore there is a built in function called `len()`. Check this out:
```py
str1 = "hello world"
print(len(str1)) # output is 11
```
Shouldn't be 10 right? well the space between hello and world is also been counted. It determines the lenght of the strings.

## Multiline Strings
PEP 8 style guide recommends that each of the line of python code contain no more than 79 characters including spaces. A multiline string in Python is a string that spans multiple lines. You can create it using triple quotes, either ''' (three single quotes) or """ (three double quotes). This allows you to include line breaks directly in the string without using special characters.

```py
str1 = """This is a multiline string.
It can span multiple lines.
You can include line breaks easily."""
```
### Note about multiline string:- 
> Line Breaks: The string retains the line breaks as you enter them. So, if you have line breaks in your multiline string, they will appear when you print it.
> Preserving Spaces: Any spaces or indentation you add in the string will be preserved.


# Docstring
It is a triple quoted string literal placed at the top of the function body. Docstrings are used to document what a function does and what kinds of parameters it expected.
```py
def my_function():
    """
    This function does something interesting.
    It takes no parameters and returns nothing.
    """
    pass  # Function implementation goes here

print(my_function.__doc__)  # Prints the docstring of the function
```

## String: Concatenation
It joins two strings together by using + operator
```py
str1 = "abdullah"
str2 = "ke 12 bacche"
print("concatenation:", str1 + str2)
```

# String: Indexing
