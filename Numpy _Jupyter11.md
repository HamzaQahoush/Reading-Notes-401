# Read: Class 11

## What is Jupyter Lab ?
* **JupyterLab** is an open-source web application primarily designed to provide a user interface  based on **Jupyter Notebook**.It enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner. 
* Some of the important features of JupyterLab :
 1. Code Console acts as scratchpad for running code interactively.
   It has full support for rich output and can be linked to a notebook kernel to log notebook activity.

 2. Any text file (Markdown, Python, R, LaTeX, etc.) can be run interactively in any Jupyter kernel.

 3. Notebook cell output can be shown into its own tab, or along with the notebook, enabling simple dashboards with interactive controls backed by a kernel.

 4. Live editing of document reflects in other viewers such as editors or consoles. 
  It is possible to have live preview of Markdown, Delimiter-separated Values, or Vega/Vega-Lite documents.

* JupyterLab can handle many file formats (images, CSV, JSON, Markdown, PDF etc.).It also displays rich output in these formats. JupyterLab provides customizable keyboard shortcuts uses key maps from many well-known text editors.

## NumPy Tutorial: Data Analysis with Python :
* NumPy is the fundamental package for array computing with Python.
* With NumPy, we work with multidimensional arrays.In n a NumPy array, the number of dimensions is called the rank, and each dimension is called an axis.
* We can create a NumPy array using the **numpy.array** function.
* One of the limitations of NumPy is that all the elements in an array have to be of the same type.
* We can check the number of rows and columns in our data using the **shape** property of NumPy arrays. 
* We can create an array where every element is zero using **numpy.zeros**.
* We can create an array where each element is a random number using **numpy.random.rand**.
* NumPy is zero-indexed, meaning that the index of the first row is 0, and the index of the first column is 0.
*  (:). A colon indicates that we want to select all the elements from the starting index up to but not including the ending index.
* We can use indexing to assign values to certain elements in arrays.
* We can find the data type of a NumPy array by accessing the **dtype** property.
* We can use the **numpy.ndarray.astype** method to convert an array to a different type. The method will actually copy the array, and return a new array with the specified data type. 
* NumPy makes it simple to perform mathematical operations on arrays. This is one of the primary advantages of NumPy, and makes it quite easy to do computations.
* Unless the arrays that you’re operating on are the exact same size, it’s not possible to do elementwise operations. In cases like this, NumPy performs **broadcasting** to try to match up elements. Essentially, broadcasting involves a few steps:
  * The last dimension of each array is compared.
    - If the dimension lengths are equal, or one of the dimensions is of length 1, then we keep going.
    - If the dimension lengths aren’t equal, and none of the dimensions have length 1, then there’s an error.
  * Continue checking dimensions until the shortest array is out of dimensions.

* In addition to the common mathematical operations, NumPy also has several methods that you can use for more complex calculations on arrays. An example of this is the **numpy.ndarray.sum** method. This finds the sum of all the elements in an array.
* There are several other methods that behave like the sum method, including:
  * **numpy.ndarray.mean** — finds the mean of an array.
  * **numpy.ndarray.std** — finds the standard deviation of an array.
  * **numpy.ndarray.min** — finds the minimum value in an array.
  * **numpy.ndarray.max** — finds the maximum value in an array.

* NumPy makes it possible to test to see if rows match certain values using mathematical comparison operations like <, >, >=, <=, and ==.
* We can change the shape of arrays while still preserving all of their elements. This often can make it easier to access array elements. The simplest reshaping is to flip the axes, so rows become columns, and vice versa. We can accomplish this with the **numpy.transpose** function.
* We can use the **numpy.ravel** function to turn an array into a one-dimensional representation. It will essentially flatten an array into a long sequence of values.
* We can use the **numpy.reshape** function to reshape an array to a certain shape we specify.

* ***Useful reference*** : [link](https://numpy.org/doc/stable/reference/arrays.ndarray.html)




