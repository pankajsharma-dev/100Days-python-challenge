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

** Convert decimal into binary, hexadecimal and octal (Day02 >> decimaltoother_test.py)

```
a=20
binary_num = bin(a)
hex_num = hex(a)
oct_num = oct(a)

print(binary_num)
print(hex_num)
print(oct_num)
```

** Math Operations (Day02 >> Mathoperaions_test.py) : check the specified file and check the comment.
PEMDAS :  Parentheses, Exponents, Multiplication/Division, Addition/Subtraction

### Assignment : BMI Calculator

Check BMI_Calculator_Assignment.py file and check the comment.

## Day 3

### Control Flow, Logical operators and Scope

Syntax of If else

```
	if condition:
		do this
	else:
		do this
```



Example 1: Simple Login System

> Create a program to demonstrate the Login functionality. If user name is "admin" and password is "password123" show Login Successful, otherwise show invalid username or password.

- work on LoginAssignment.py file. 

Example 2: Purchase Discount use case

> Create an application to show the final amount need to be paid after discount. Follow inputs provided in PurchaseDiscount.py file

- Work on PurchaseDiscount.py file
- Read the instruction properly.

Example 3: ATM Withdraw Use case 

> Check account balance before allowing a withdrawal.

- work on ATMWithdrawCase.py file, read the comment

> Day3 Final Assignment : 

### 🍕 Python Pizza Ordering System - Assignment
This assignment will help you practice key Python concepts such as:
- User Input
- Conditional Statement(if-else)
- String function
- Loops and Disctionaries
- Basic Calculation logic

📝 Assignment Task Description
Create a Pizza Ordering System in Python with the following requirements:

📌 Features to Implement
Display the Pizza Menu

Menu should include 4 types of pizzas with their prices.
Example:
```
Margherita - ₹200
Pepperoni - ₹250
BBQ Chicken - ₹300
Veggie Delight - ₹220

```
Take User Input

Ask the user to select a pizza.
Ask for the quantity they wish to order.
Ask if they want extra cheese and extra olives (yes/no).
Order Validation

If the pizza name is not on the menu, display "❌ Invalid pizza choice." and exit the program.
Ensure quantity is a positive number; otherwise, ask again.
Price Calculation

Base price = Pizza price × Quantity
Extra Cheese = ₹30 (if selected)
Extra Olives = ₹20 (if selected)
Display Final Bill

Show the complete order summary in a user-friendly format.
Example Output:

```
🧾 Order Summary:
Pizza: Margherita x 2
Extra Cheese: Yes
Extra Olives: No
Total Amount to Pay: ₹430

```
Bonus Features (Optional for Extra Practice)

Offer a combo discount if total bill exceeds ₹1000 (e.g., 10% off).
Ask for user details like name and phone number for better interaction.

Learning Outcome
By completing this assignment, you'll gain practical experience in:

✔️ Handling multiple conditions with if-else
✔️ Using strip() and lower() for better input handling
✔️ Building a simple yet effective billing system
✔️ Improving code readability with meaningful variable names and comments

Challenge
Once your basic version is complete, try adding:
🔹 A combo offer for orders above ₹1000
🔹 An option for home delivery with delivery charges