# Forms

An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server.
Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data,
including text boxes, checkboxes, radio buttons, date pickers and so on. Forms are also a relatively 
secure way of sharing data with the server, as they allow us to send data in POST requests with cross-site request forgery protection.


## Declaring a Form
The declaration syntax for a Form is very similar to that for declaring a Model, and shares the same field types (and some similar parameters). 

we need to import forms `from django import forms`

### Form fields
There are many other types of form fields, which you will largely recognize from their similarity to the equivalent model field classes: BooleanField, CharField, ChoiceField, TypedChoiceField, DateField, DateTimeField, DecimalField, DurationField, EmailField, FileField, etc 
