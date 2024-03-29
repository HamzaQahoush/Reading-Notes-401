
## Python Scope & the LEGB Rule: 

* The concept of **scope** rules how **variables** and **names** are looked up in your code. It determines the visibility of a variable within the code. The scope of a name or variable depends on the place in your code where you create that variable. The Python scope concept is generally presented using a rule known as the **LEGB rule** **"stand for Local, Enclosing, Global, and Built-in scopes"**.
  * **Local (or function) scope** is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function. These names will only be visible from the code of the function. It’s created at function call, not at function definition, so you’ll have as many different local scopes as function calls. This is true even if you call the same function multiple times, or recursively. Each call will result in a new local scope being created.

  * **Enclosing (or nonlocal) scope** is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. This scope contains the names that you define in the enclosing function. The names in the enclosing scope are visible from the code of the inner and enclosing functions.

  * **Global (or module) scope** is the top-most scope in a Python program, script, or module. This Python scope contains all of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.

  * **Built-in scope **is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python. Names in this Python scope are also available from everywhere in your code. It’s automatically loaded by Python when you run a program or script.

* The two general types of scopes :
 + **Global scope**: The names that you define in this scope are available to all your code.
 + **Local scope**: The names that you define in this scope are only available or visible to the code within the scope.

* A Python scope determines where in your program a name is visible. Python scopes are implemented as **dictionaries** that map names to objects. These dictionaries are commonly called **namespaces**. These are the concrete mechanisms that Python uses to store names. They’re stored in a special attribute called .__dict__.


* the **global** statement can be used to modify global names from almost any place in your code, as you’ll see in The global Statement. Modifying global names is generally considered bad programming practice because it can lead to code that is:
  1. **Difficult to debug**: Almost any statement in the program can change the value of a global name.
  2. **Hard to understand**: You need to be aware of all the statements that access and modify global names.
  3. **Impossible to reuse**: The code is dependent on global names that are specific to a concrete program.
* Good programming practice recommends using local names rather than global names. Here are some tips:
 + Write self-contained functions that rely on local names rather than global ones.
 + Try to use unique objects names, no matter what scope you’re in.
 + Avoid global name modifications throughout your programs.
 + Avoid cross-module name modifications.
 + Use global names as constants that don’t change during your program’s execution.

* Similarly to global names, nonlocal names can be accessed from inner functions, but not assigned or updated. If you want to modify them, then you need to use a **nonlocal statement**. With a nonlocal statement, you can define a list of names that are going to be treated as nonlocal.

* **A closure** is an inner or nested function that carries information about its enclosing scope, even though this scope has completed its execution.
 - **Note**: You can also call this kind of function **a factory**, a factory function, or—to be more precise—a closure factory to specify that the function builds and returns closures (an inner function), rather than classes or instances.
* **vars()** is a Python built-in function that returns the .__dict__ attribute of a module, class, instance, or any other object which has a dictionary attribute.
* **dir()** : You can use dir() without arguments to get the list of names in the current Python scope. If you call dir() with an argument, then the function attempts to return a list of valid attributes for that object
