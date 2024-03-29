Read: Class 19 Automation Summary
## Python Regular Expression
* Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not. If you've ever used search engines, search and replace tools of word processors and text editors - you've already seen regular expressions in use. They are used at the server side to validate the format of email addresses or passwords during registration, used for parsing text data files to find, replace, or delete certain string, etc. They help in manipulating textual data, which is often a prerequisite for data science projects involving text mining.

* In Python, regular expressions are supported by the re module. That means that if you want to start using them in your Python scripts, you have to import this module with the help of import:**import re**
* The re library in Python provides several functions that make it a skill worth mastering.
* **Wild Card Characters: Special Characters**:
 * Special characters are characters that do not match themselves as seen but have a special meaning when used in a regular expression. For simple understanding, they can be thought of as reserved metacharacters that denote something else and not what they look like.
 * This is helpful if you want to make sure a document/sentence ends with certain characters.
```
re.search(r'cake$', "Cake! Let's eat cake").group()
'cake'
## The next search will return the NONE value, try it:
# re.search(r'cake$', "Let's get some cake on our way home!").group()
```
 * [abc] - Matches a or b or c.
 * [a-zA-Z0-9] - Matches any letter from (a to z) or (A to Z) or (0 to 9).

![](https://miro.medium.com/max/3640/1*9rlD7grrXfk301gCa7XSMw.png)

## Automation Using Python
* You can automate nearly everything with Python. From sending emails and filling out PDFs and CSVs to interacting with external APIs and sending HTTP requests. Whatever your idea, it’s more than likely that you can pull it off using Python along with its modules and tools.

## shutil — High-level File Operations
* The shutil module includes high-level file operations such as copying and archiving.
1. **Copying Files**
  -  copyfile() copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file.
  - The copy() function interprets the output name like the Unix command line tool cp. If the named destination refers to a directory instead of a file, a new file is created in the directory using the base name of the source.



## Watchdog
* **Watchdog** is a python API library and shell utilities to *monitor file system events*.
* Directory monitoring made easy with across-platform API and a shell tool to run commands in response to directory changes.
* We can use pip to install watchdog quickly and easily: $ pip install watchdog.

