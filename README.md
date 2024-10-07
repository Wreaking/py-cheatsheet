# Chapter2: Understanding the variables
Let us understand what are the variables and the additional cases.
```py
a = "hello there"
print(a)
b = 10
print(b)
c = 1.3
print(c)
```
These are the basic code lines. Let's understand in simple language.

> "a" is your **variable** which acts like a memeory storage
> 
> "=" is your **assignment operator** not equal. An operator is a symbol like =, +, -, / etc. that performs some operation on one or more values
> 
> "hello there", "10", "1.3" are your values. Those values are stored in a , b , c variables which acts like a memory storage

how do we say the line code in physical conversation?
We say,
> Declare a variable ***a*** is assign to a value(string) "hello world" and print a
> 
> Declare a variable ***b*** is assign to a value(integer) 10 and print b
> 
> Declare a variable ***c*** is assign to a value(float) 1.3 and print c

Easy right? Try to complete a problem in codetantra 3.1.1

Let us understand more deeper with different situations...
## Case1:
D
Consider a code line
```py
a b c = "hello"
```
![image](https://github.com/user-attachments/assets/3351c1e5-95cf-46e5-95af-5593b7e40e73)

You would get a syntax error. In Python, variable assignments must be formatted properly. The correct way to assign the value 10 to a multiple variables would be to use commas to separate the variable names;
```py
a, b, c = 10, 12, 15
```
here,
> ***a*** is assign to a value 10
> 
> ***b*** is assign to a value 12
> 
> ***c*** is assign to a value 15

## Case2:
assigning more than one variable to one value.
```py
a = b = c = 2
```
In this code you are assigning(a, b, c) to a value 2, that means
> Declare a variable ***a*** is assigned to value 2
> 
> Declare a variable ***b*** is assigned to value 2
> 
> Declare a variable ***c*** is assigned to value 2

## Case3:
Swapping the values:
```py
a = 30
b = 40

a, b = b, a #ouput of a and b are 40 and 30 
```
In this code, we are swapping the values in the two variables, i.e
> the original values of a and b are 30 and 40
> 
> We had swapped the values which means,
> 
> - a = b and b = a
> - 
> - the value of b(40) is given to variable a and value of a(30) is given to b

Hope you got it.Try to solve the problem number 3.1.6 in codetantra


