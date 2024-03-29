# Read: Class 04 summary:

## Classes and Objects
* Objects are created using classes, which are actually the focal point of **OOP**.
* The class describes what the object will be, but is separate from the object itself. In other words, a class can be described as an object's blueprint, description, or definition.
* The __init__ method is the most important method in a class.
This is called when an instance (object) of the class is created, using the class name as a function.

* All methods must have **self** as their first parameter, although it isn't explicitly passed, Python adds the self argument to the list for you; you do not need to include it when you call the methods. Within a method definition, self refers to the instance calling the method.

```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

myobjectx.variable
```
* You can create multiple different objects that are of the same class (have the same variables and functions defined). However, each object contains independent copies of the variables defined in the class.

## Thinking Recursively in Python:
* A recursive function is a function defined in terms of itself via self-referential expressions.
* All recursive functions share a common structure made up of two parts: base case and recursive case.
* A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure. 

## Python Testing with pytest: Fixtures and Coverage:
* fixtures are when you want to have some objects available to all of your tests. Those objects might contain data you want to share across tests.

* coverage is a package that will create a report with every part of the python library that your program used.
