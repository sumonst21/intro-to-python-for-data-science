# Functions and Packages

To leverage the code that brilliant Python developers have written, you'll learn about using functions, methods and packages. This will help you to reduce the amount of code you need to solve challenging problems!

## Table of Contents

[Functions](#functions)  
[Familiar functions](#familiar-functions)  
[Help!](#help)  
[Multiple arguments](#multiple-arguments)  
[Methods](#methods)  
[String Methods](#string-methods)  
[List Methods](#list-methods)  
[List Methods (2)](#list-methods-2)  
[Packages](#packages)  
[Import package](#import-package)  
[Selective import](#selective-import)  
[Different ways of importing](#different-ways-importing)  

### Functions

A function is a block of code which only runs when it is called.
You can pass data, known as parameters, into a function.
A function can return data as a result.

### Familiar functions

Out of the box, Python offers a bunch of built-in functions to make your life as a data scientist easier. You already know two such functions: [print()](https://docs.python.org/3/library/functions.html#print) and [type()](https://docs.python.org/3/library/functions.html#type). You've also used the functions [str()](https://docs.python.org/3/library/functions.html#func-str), [int()](https://docs.python.org/3/library/functions.html#int), [bool()](https://docs.python.org/3/library/functions.html#bool) and floa[t()](https://docs.python.org/3/library/functions.html#float) to switch between data types. These are built-in functions as well.

Calling a function is easy. To get the type of `3.0` and store the output as a new variable, `result`, you can use the following:

```py
result = type(3.0)
```

The general recipe for calling functions and saving the result to a variable is thus:

```py
output = function_name(input)
```

 > Code example added on script.py

`The [len()](https://docs.python.org/3/library/functions.html#len) function is extremely useful;`

### Help"&#33;"

Maybe you already know the name of a Python function, but you still have to figure out how to use it. Ironically, you have to ask for information about a function with another function: [help()](https://docs.python.org/3/library/functions.html#help). In IPython specifically, you can also use ? before the function name.

To get help on the [max()](https://docs.python.org/3/library/functions.html#max) function, for example, you can use one of these calls:

```py
help(max)
?max
```

Use the Shell on the right to open up the documentation on [complex()](https://docs.python.org/3/library/functions.html#complex). Which of the following statements is true?

#### Possible Answers

- [ ] complex() takes exactly two arguments: real and [, imag].  
- [ ] complex() takes two arguments: real and imag. Both these arguments are required.  
- [x] complex() takes two arguments: real and imag. real is a required argument, imag is an optional argument.  
- [ ] complex() takes two arguments: real and imag. If you don't specify imag, it is set to 1 by Python.

### Multiple Arguments

In the previous exercise, the square brackets around `imag` in the documentation showed us that the `imag` argument is optional. But Python also uses a different way to tell users about arguments being optional.

Have a look at the documentation of [sorted()](https://docs.python.org/3/library/functions.html#sorted) by typing `help(sorted)` in the IPython Shell.

You'll see that [sorted()](https://docs.python.org/3/library/functions.html#sorted) takes three arguments: `iterable`, `key` and `reverse`.

`key=None` means that if you don't specify the `key` argument, it will be `None`. `reverse=False` means that if you don't specify the `reverse` argument, it will be `False`.

In this exercise, you'll only have to specify `iterable` and `reverse`, not `key`. The first input you pass to [sorted()](https://docs.python.org/3/library/functions.html#sorted) will be matched to the `iterable` argument, but what about the second input? To tell Python you want to specify `reverse` without changing anything about `key`, you can use `=`:

```py
sorted(___, reverse = ___)
```

Two lists have been created for you on the right. Can you paste them together and sort them in descending order?

Note: For now, we can understand an [iterable](https://docs.python.org/2/glossary.html#term-iterable) as being any collection of objects, e.g. a List.

### Methods

#### Build-in Functions

- Maximum of list: max()
- Length of list or string: len()
- Get index in list: ?
- Reversing a list: ?

[Link to the video on my course](https://campus.datacamp.com/courses/intro-to-python-for-data-science/chapter-3-functions-and-packages?ex=5)

> Methods: Functions that belongs to objects

##### Example of Methods

- capitalize()  replace()
- bit_length()  conjugate()
- index()   count()

```txt
In Python Everything is Object and each object have spacific methods associated, depending on the type
```

### String Methods

### List Methods 2

### Packages

### Import Package

### Selective Import

### Different Ways of Importing