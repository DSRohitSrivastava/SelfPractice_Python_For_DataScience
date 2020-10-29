# Python for DataScience




<p align="right">- By Rohit Srivastava
 <img src="https://raw.githubusercontent.com/QARohitSrivastava/gitHub/main/Rohit%20Srivastava%20Logo.jpg" width="125" height="125" title="Rohit Srivastava" alt = "Rohit Srivastava" />
</p>




A python script can be written in python interactive shell or in the code editor. A python file has an extension .py.

### Python Indentation

An indentation is a white space in a text. Indentation in many languages is used to increase code readability, however python uses indentation to create block of codes. In other programming languages curly brackets are used to create blocks of codes instead of indentation. One of the common bugs when writing python code is wrong indentation.

![Indentation Error](./images/indentation.png)

### Comments

Comments are very important to make the code more readable and to leave remarks in our code. Python doesn't run comment parts of our code.
Any text starting with hash(#) in python is a comment.

**Example: Single Line Comment**

```shell
    # This is the first comment
    # This is the second comment
    # Python is eating the world
```

**Example: Multiline Comment**

Triple quote can be used for multiline comment if it is not assigned to a variable

```shell
"""This is multiline comment
multiline comment takes multiple lines.
python is eating the world
"""
```

### Data types

In python there are several types of data types. Let's get started with the most common ones. Different data types will be covered in detail in other sections. For the time being let us just go through the different data types and get familiar with them. You do not have to have a clear understanding now.

#### Number

- Integer: Integer(negative, zero and positive) numbers
  Example:
  ... -3, -2, -1, 0, 1, 2, 3 ...
- Float: Decimal number
  Example
  ... -3.5, -2.25, -1.0, 0.0, 1.1, 2.2, 3.5 ...
- Complex
  Example
  1 + j, 2 + 4j

#### String

A collection of one or more characters under a single or double quote. If a string is more than one sentence then we use a triple quote.

**Example:**

```py
'Rohit'
'Srivastava'
'Python'
'I love teaching'
'I hope you are enjoying Python for Everyone'
```

#### Booleans

A boolean data type is either a True or False value. T and F should be always uppercase.

**Example:**

```python
    True  #  Is the light on? If it is on, then the value is True
    False # Is the light on? If it is off, then the value is False
```

#### List

Python list is an ordered collection which allows to store different data type items. A list is similar to an array in JavaScript.

**Example:**

```py
[0, 1, 2, 3, 4, 5]  # all are the same data types - a list of numbers
['Banana', 'Orange', 'Mango', 'Avocado'] # all the same data types - a list of strings (fruits!)
['Noida','Lucknow', 'New Delhi','Jaipur'] # all the same data types - a list of strings (countries!)
['Banana', 10, False, 9.81] # different data types in the list - string, integer, boolean and float
```

#### Dictionary

A python dictionary object is an unordered collection of data in a key:value pair format.

**Example:**

```py
{'name':'Rohit', 'country':'India', age:250, 'is_married':True}
```

#### Tuple

A tuple is an ordered collection of different data types like list but tuples can not be modified once they are created. They are immutable.

**Example:**

```py
('Rohit', 'Book', 'Pen', 'Mouse')
```

#### Set

A set is a collection of data types similar to list and tuple. Unlike list and tuple, set is not an ordered collection of items. Like in mathematics, set in python stores only unique items.

In later sections, we will go in detail about each and every python data type.

**Example:**

```py
{3.14, 9.81, 2.7} # order is not important in set
```

<h1 align="center" style="color:#306998;font-size:64px;">PYTHON DATA TYPES</h1>

Different data types in python. There are different data type in python programming. To identify the data tpe we use the type method.
```


## Strings

String is data type. Any data under single or double quot are a string. There are diferent string methods to deal with string data types. To check the length of a string use the **_len()_** method.

```py
# Assigning variables to string value

first_name = "Rohit"
space = ' ' # an empty space string
last_name = "Srivastava"
country = "India"
full_name = ' Rohit Srivastava'
```

```py
print(first_name)
print(len(first_name))
print(last_name)
print(len(last_name))
print(country)
print(space)  # You don't see the printed empty space
print(full_name) # there is indent because of the trailing space in the full name is string

```
    Rohit
    5
    Srivastava
    10
    India

     Rohit Srivastava

### String Concatination

Merging two or more strings together is called **_concatination_**

```python

# String concatination
first_name = "Rohit"
space = ' ' # an empty space string
last_name = "Srivastava"
country = "India"
city = 'Noida'
full_name = first_name  + space + last_name
git_repo= 'Python ' + ' for ' + ' Everyone'
person_info = 'I am ' + full_name + '. I live in ' + country + ', '+ city + '.'
print('Full name: ', full_name)
print('Person Information:', person_info)
print('Git repository: ', git_repo)


```

    Full name:  Rohit Srivastava
	Person Information: I am Rohit Srivastava. I live in India, Noida.
	Git repository:  Python  for  Everyone

### String transformations

- **_s.lower()_**: Change all letters to lowercase
- **_s.upper()_**: Change all letters to uppercase
- **_s.capitalize()_**: Change all letters to capitalcase
- **_s.title()_**: Change to titlecase
- **_s.swapcase()_**: Change all uppercase letters to lowercase, and vice versa

```python
firstName = 'Rohit'
lastName = 'Srivastava'
space = ' '
full_Name = first_name + space + last_name;


```py
	# Changing string to lower case
	print('=== change to lower case ===')
	print(first_name.lower())
	print(last_name.lower())
	print(full_Name.lower())

```py

    === change to lower case ===
    rohit
    srivastava
    rohit srivastava
	

# Changing string to upper case
print('=== change to upper case ===')
print(first_name.upper())
print(lastName.upper())
print(full_Name.upper())

```

    === change to upper  case ===
    ROHIT
    SRIVASTAVA
    ROHIT SRIVASTAVA

# Changing string to capitalize
print('=== change to capitalize ===')
print(first_name.capitalize())
print(lastName.capitalize())
print(full_Name.capitalize())


```

    === change to capitalize ===
    Rohit
    Srivastava
    Rohit srivastava
	
	

# Changing string to capitalize

print('=== change to title ===')
title = 'python for everyone'
sub_title = 'learning programming using python'
lang = 'python'
level = 'both begineer and advanced learners'
print(title.title())
print(sub_title.title())
print(lang.title())
print(level.title())


```

    === change to title  ===
    Python For Everyone
    Learning Programming Using Python
    Python
	Both Begineer And Advanced Learners

	
	

# Changing string to swapcase()
print('=== swapping cases ===')

first_name = 'Rohit'
last_name = 'Srivastava'
space = ' '
full_name = first_name + space + last_name;

print(first_name.swapcase())
print(last_name.swapcase())
print(full_name.swapcase())




```

    === swapping cases ===
    rOHIT

    sRIVASTAVA

    rOHIT sRIVASTAVA


### Spliting string

Empty space is the default paramter.

- **_s.split()_**: Change the string to a list containing the string
- **_s.split(' ')_**:Change the string to a list containing the words of in the string
- **_s.split(',')_**: split the words at the comma

```python
# Spliting a stirng to list
first_name = 'Rohit'
last_name = 'Srivastava'
full_name = 'Rohit Srivastava'
programming_lang = 'python, R, matlab, and Java'


# Changing a string to list
print(first_name.split())
print(list(first_name))
print(full_name.split(' '))
print(programming_lang.split(','))


# To check the length of string
print(len(first_name))

# To check the data type of the string
print(type(first_name))
```

    ['Rohit']
	['R', 'o', 'h', 'i', 't']
	['Rohit', 'Srivastava']
	['python', ' R', ' matlab', ' and Java']
    5
    <class 'str'>

#### String Formatting

### Exercises- Strings

1. Concatinate the string 'Python', 'For','Everyone' to a single string, 'Python for Everyone'
1. Concatinate the string 'Coding', 'For' , 'All' to a single string, 'Coding For All'
1. Declare a variable name company and assign it to an initial value **"Coding For All"**.
1. Print company using **print()**
1. Print the **length** of the company string using **_len()_** method and _print()_
1. Change all the string to capital letters using **upper()** method
1. Change all the string to lowercase letters using **lower()** method
1. Use **_capitalize(),title(), swapcase()_** methods to format the value stored in the varaible name company
1. Cut(slice) out the first word of the company string
1. Check if the string contains a word **Coding** using the method index, find or other methods.
1. Replace the word coding in the string 'Coding For All' to Python using replace or other methods.
1. Change Python for Everyone to Python for All using the replace method or other methods
1. Split the string 'Coding For All' at the space using **split()** method
1. "Facebook, Google, Microsoft, Apple, IBM, Oracle, Amazon" **split** the string at the comma
1. What is character at index 10 in "Coding For All"
1. Create an acronym or an abbrivaton for the name 'Python For Everyone'
1. Create an acronym or an abbrivaton for the name 'Coding For All'
1. Use **index** to determine the position of the first occurrence of C in Coding For All
1. Use **index** to determine the position of the first occurrence of F in Coding For All
1. Use **rfind** to determine the position of the last occurrence of l in Coding For All People.
1. Use **index or find** to find the position of the first occurrence of the word **because** in the following sentence:**'You cannot end a sentence with because because because is a conjunction'**
1. Use **rindex** to find the position of the last occurrence of the word **because** in the following sentence:**'You cannot end a sentence with because because because is a conjunction'**
1. Slice out the phase **because because because** in the following sentence:**'You cannot end a sentence with because because because is a conjunction'**
1. Use **search** to find the position of the first occurrence of the word **because** in the following sentence:**'You cannot end a sentence with because because because is a conjunction'**
1. Slice out the phase **because because because** in the following sentence:**'You cannot end a sentence with because because because is a conjunction'**
1. Use **trim()** to remove if there is trailing whitespace at the beginning and the end of a string.E.g " Coding For All ".
1. Use **startswith()** method with the string Coding For All make the result true
1. Use **endswith()** method with the string Python for Everyone make the result true



<BR>