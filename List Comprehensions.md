
## List Comprehensions in Python
* **List comprehensions** provide a concise way to create lists.It consists of brackets containing an expression followed by a for clause, then zero or more for or if clauses. The expressions can be anything, meaning you can put in all kinds of objects in lists.
* The list comprehension always returns a result list.
* The list comprehension starts with a **‘[‘** and **‘]’**, square brackets, to help you remember that the result is going to be a list.

* The basic syntax uses square brackets :
```
[ expression for item in list if conditional ]
```
* This is equivalent to:

```
for item in list:
    if conditional:
        expression
```

* **Example** :
* Print numbers only from a given string
* This example show how to extract all the numbers from a string.

```
string = "Hello 12345 World"
numbers = [x for x in string if x.isdigit()]
print numbers
>> ['1', '2', '3', '4', '5']
```

* Change x.isdigit() to x.isalpha() if you don’t want any numbers.

## Primer on Python Decorators
* a **decorator** is a function that takes another function and extends the behavior of the latter function without explicitly modifying it.
* In Python, functions are ***first-class objects***. This means that functions can be passed around and used as arguments, just like any other object (string, int, float, list, and so on).
* It’s possible to define functions inside other functions. Such functions are called **inner functions**. 
