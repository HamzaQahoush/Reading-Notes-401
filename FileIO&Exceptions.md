# **FileIO & Exceptions**

![Image](https://files.realpython.com/media/Reading-and-Writing-Files-in-Python_Watermarked.0d394921fd90.jpg)

## **What Is a File?**
>  At its core, a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

## it consist of three main parts:

**Header:** metadata about the contents of the file (file name, size, type, and so on)

**Data:** contents of the file as written by the creator or editor

**End of file (EOF):** special character that indicates the end of the file

### Opening and Closing a File in Python : 
`file = open('dog_breeds.txt')` 

we should always make sure that an open file is properly closed.

`with open('dog_breeds.txt') as reader:`
  
The with statement automatically takes care of closing the file once it leaves the with block, even in cases of error. 



## **Reading Files**
![Image](https://www.netclipart.com/pp/m/145-1457211_gopher-png-source-https-github-gopher-gopher-svg.png)


> These are the methods used in reading files
> - `.read(size=-1)` :  reads from the file based on the number of size bytes, if the value less than 0 or not entered it will read the whole file 
> - `.readline(size=-1)`: same as the above but for the lines 
> - `.readlines()` :  reads the rest of the lines and return them as a list 


## **Writing Files**

> These are the methods used in writing files
  > - `.write(string)`  :  This writes the string to the file. 
  > - `.writelines(seq)` :  This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you 
