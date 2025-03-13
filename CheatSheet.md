# Python 100 Days Challenge - CheatSheet

## Day 1

### Printing a simple "welcome in python" String on console

```
print("Welcome in Python")
```

### Taking the user Input
> Use the input() function to take user input. (Refer :  Day01 >> input_task.py file)

### Variable

A variable give a name to a piece of data.Like a box with a label, it tells you what is inside the box.

> Create a program to accept a greeting message, show the greeting message along with total number of characters present in message.  (Refer :  Day01 >> variable_task.py file)

### Variable Naming Rules

1. Make sure your variable names are descriptive
2. Don't have spaces between words
3. Don't start with numbers
4. Don't use special words like print or input
5. Choose simple words that are less likely to become typos
6. Check the company style guidelines if you start work at a company
-----
### Assignment Time

1. Assignment: Personalized Greeting Card Generator

Concepts Covered: print(), input(), string concatenation

Task:

Ask the user for their name and favorite color.
Generate a personalized greeting card message that includes a fun design using special characters.

** Sample Output:

```
*****************************
*      HAPPY BIRTHDAY!      *
*****************************
Hello Priya! 
- Wishing you a fantastic day filled with joy and laughter.
- Here's something special in your favorite color, Blue!
```
-----
2. Assignment: Temperature Conversion Tool

Concepts Covered: input(), variable usage, string formatting

Task:

- Ask the user to enter a temperature in Celsius.
- Convert it to Fahrenheit using the formula: F = (C × 9/5) + 32
- Display the result in a clear, user-friendly message.

** Sample Output:

```
Enter temperature in Celsius: 30
30°C is equal to 86°F
```
-----
3. Assignment: Username Generator

Concepts Covered: String slicing, concatenation, .upper(), .lower()

Task:

- Ask the user for their first name, last name, and birth year.
- Generate a fun username using a combination of these details.

** Sample Output:

```
Enter your first name: Rahul
Enter your last name: Sharma
Enter your birth year: 1999
Your unique username is: RSHARMA99
```

Hint: Combine initials + last name + last two digits of the birth year.
-----
4. Assignment: Word Counter for Essays

Concepts Covered: String manipulation, .split(), .strip()

Task:

- Ask the user to enter a paragraph of text.
- Count the total number of words, characters, and sentences in the paragraph.

** Sample Output:

```
Enter your essay: Python is amazing. It makes coding fun!
Word Count: 8
Character Count: 43
Sentence Count: 2
```
-----

5. Assignment: Secret Code Generator

Concepts Covered: .replace(), .lower(), .upper()

Task:

- Ask the user for a message.
- Replace vowels with special characters:
	- a → @, e → 3, i → 1, o → 0, u → µ
- Display the encoded message.

** Sample Output:

```
Enter your message: Hello World
Secret Code: H3ll0 W0rld
```

## Day 2

### Primitive Data Types, Numbers, Operations, Type Conversions, f-Strings

Primitive data types in Python are the most basic types of data. They are the building blocks for data manipulation in Python and are typically immutable, 
meaning their value cannot change after they are created. Here are the main primitive data types in Python:

Examples of Primitive Data Types

- Integer (int) :
	- Represents whole numbers.
	- Example: x = 10
	
- Float (float) :
	- Represents floating-point numbers (decimal values).
	- Example: y = 10.5
	
- Boolean (bool) :
	- Represents True or False values.
	- Example: is_active = True
	
- String (str) :
	- Represents a sequence of characters.
	- Example: name = "Pankaj Sharma"
	
```
x = 10              # Integer
y = 10.5            # Float
is_active = True    # Boolean
name = "Pankaj Sharma"      # String

print(type(x))      
print(type(y))     
print(type(is_active))  
print(type(name))   

```

** Examples

1. Open Day02 >> datatype_task.py (Read Comment and complete)


### Type Conversion in python

Type conversion is basically converting one type into another type. 
There are two types of Type Conversion in python:

1. Implicit Type Conversion
2. Explicit Type Conversion

In Implicit type conversion of data types in Python, the Python interpreter automatically converts one data type to another without any user involvement.

** Example of Implicit Type Conversion (Day02 >> typeconvertion_test.py)

```
a=10
b=1.5
c=a+b
print(c)
d=True
e=a+d
print(e)
```

** Example of Explicit Type Conversion part1 (Day02 >> explicittypeconvertion_test.py)

```
strNumber = "135"
x=5+int(strNumber)
f = float(x)
print(x)
print(f)
```

** Example of Explicit Type Conversion part2 (Day02 >> explicittypeconvertion2_test.py)

```
msg="hello world"
print(list(msg))
print(tuple(msg))
print(set(msg))
```