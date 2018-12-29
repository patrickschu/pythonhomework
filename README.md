### Object Oriented Programming Homework

The goal of the exercise below is to run code over a couple of books to do word counts, find out which book is the longest, etc. 

High level goals:

1. create a class `Book`

2. create attributes and functions to interact with books

3. read in a sample of books from Proj Gut and run basic analytics on text length and such


General reqs:

Please try to 
follow either the official [Python style guidelines]( https://www.python.org/dev/peps/pep-0008/)
or the [Google Python Style guide](https://google.github.io/styleguide/pyguide.html)


### Exercises 

Use [oop.py](https://github.com/patrickschu/pythonhomework/blob/master/oop.py)
(Instructions below are identical to what you find in oop.py, where they are more readable)

EX 1. Define a class `Book`.  
 --> Read this doc for guidance: https://docs.python.org/3/tutorial/classes.html#class-objects


Book takes the following inputs:

`file_name` (str), the name of the file the book is stored in
`content`  (str), the text of the book
`uniq_id` (int), a unique number we assign to each book


EX 1 Extra Credit: Make sure `Book` inherits from `object`.
 --> https://docs.python.org/3/tutorial/classes.html#inheritance


EX 2. Adding methods
Test the Book class on some random input to make sure it works, i.e.  come up with a made up file_name, content, etc and initialize a Book object

Implement the following two methods:

- file_type , a method that returns the type of text file that has been read in. 
--> You can use os.path.splitext on `file_name` for this: https://docs.python.org/2/library/os.path.html#os.path.splitext

- compute_length , a method that returns the length of `content` in characters


EX 3. Use Book class

Read the files in *book_samples.zip* into Python and create a Book object for each. 

Test out the functions implemented above for correctness. 
