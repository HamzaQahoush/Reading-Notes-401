## What is Django?
Django is a high-level Python Web framework that encourages rapid development and clean pragmatic design.

A Web framework is a set of components that provide a standard way to develop websites fast and easily.
Django’s primary goal is to ease the creation of complex database-driven websites.
Some well known sites that use Django include PBS, Instagram, Disqus, Washington Times, Bitbucket and Mozilla.

Getting started with Django :

1. Install Django : 
`py -m pip install Django` after creating directory environment 

2. Creating a project :
 From the command line, cd into a directory where you’d like to store your code, then run the following command:
 ` django-admin startproject mysite`
 
The output of  what startproject created:


 ![](https://i.ibb.co/WH9c4z2/dianji.png)
 
 ![](https://i.ibb.co/FXC9t9h/files.png)
 
 3.  The development server :
 `py manage.py runserver`
By default, the runserver command starts the development server on the internal IP at port 8000.

If you want to change the server’s port, pass it as a command-line argument. For instance, this command starts the server on port 8080: `py manage.py runserver 8080`



