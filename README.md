# Python Tutorial By - Datascience ki Baatein

## Why We Use Python + Its Role in Data Science
Python has become one of the most popular programming languages. Here's why:
### ✅ 1. Easy to Learn & Read

•	Simple syntax (close to English).

•	Great for beginners and pros alike.
### Example: Hello World
```
print("Hello, World!")
```

### ✅ 2. Versatile
•	Can be used in web development, automation, AI, data analysis, machine learning, etc.

### ✅ 3. Huge Community Support
•	Tons of tutorials, solutions, and discussions online.

### ✅ 4. Powerful Libraries
•	Rich set of libraries for every use case: data, AI, visualization, web, etc.

## Role of Python in Data Science
Python is the #1 language for Data Science. Here's how it fits into each stage:

### 📊 1. Data Collection

•	Scrape data from the web using BeautifulSoup, Scrapy.

•	Collect API data using requests.
```
import requests
response = requests.get("https://api.github.com")
print(response.json())
```
### 📈 2. Data Cleaning & Preparation
•	Use pandas and numpy to clean, filter, and preprocess data.
import pandas as pd
df = pd.read_csv("data.csv")
df.dropna(inplace=True)

### 📉 3. Data Analysis
•	Analyze trends, find patterns, and summarize data.
```
print(df.describe())
print(df.groupby("Gender")["Salary"].mean())
```

### 📊 4. Data Visualization
•	Use matplotlib, seaborn, or plotly to create graphs and dashboards.
```
import matplotlib.pyplot as plt
df['Salary'].hist()
plt.show()
```
### 🧠 5. Machine Learning
•	Use scikit-learn, TensorFlow, or PyTorch to build models.
```
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X, y)
```
### 🤖 6. Deployment
•	Deploy models via Flask, FastAPI, or cloud services (AWS, Heroku).


## Variables, Data Types, Comments & Docstrings
### 🔹 1. Variables in Python
Variables are used to store data. You don’t need to declare the type; Python figures it out.

### Syntax:
```
name = "Alice"
age = 25
height = 5.6
```
•	name is a string

•	age is an integer

•	height is a float

### Rules for Variable Names:
•	Must start with a letter or underscore _

•	Cannot start with a number

•	Case-sensitive (name ≠ Name)


### 🔹 2. Python Data Types
|Type	|Example	|Description|
|-------|-----------|-----------|
|int	|10, -3	|Whole numbers|
|float	|3.14, -7.2	|Decimal numbers|
|str	|"hello"	|Text|
|bool	|True, False	|Boolean (logical) values|
|list	|[1, 2, 3]	|Ordered, changeable collection|
|tuple	|(1, 2, 3)	|Ordered, immutable collection|
|dict	|{"name": "John"}	|Key-value pairs|
|set	|{1, 2, 3}	|Unordered, no duplicates|

### Example:
```
x = 42             # int
pi = 3.14          # float
name = "Python"    # str
is_active = True   # bool
colors = ["red", "blue", "green"]  # list
```
________________________________________
### 🔹 3. Comments in Python
Comments help explain the code. They are ignored by the interpreter.
✅ Single-line Comment:
```
# This is a comment
name = "Alice"  # This is also a comment
```
✅ Multi-line Comment (Hacky Way):
```
# This is a multi-line comment
# You can continue using #
# on every line
```
________________________________________
### 🔹 4. Docstrings (Documentation Strings)
Docstrings are multi-line strings used to describe what a function/class/module does. They’re enclosed in triple quotes (''' or """).

✅ Example:
```
def greet(name):
    """
    This function greets the user with the given name.
    """
    print(f"Hello, {name}!")
```
You can access the docstring using:
```
print(greet.__doc__)
```

## Output & Type Conversion
🔹 1. Input in Python
input() is used to take user input from the keyboard. It always returns a string.
✅ Example:
```
name = input("Enter your name: ")
print("Hello", name)
```
📝 Note:
You need to convert input to integer/float if needed (explained in type conversion below).
________________________________________
🔹 2. Output in Python
print() is used to display output.
✅ Example:
```
print("Hello, world!")
✅ Multiple Values:
name = "Alice"
age = 25
print("Name:", name, "| Age:", age)
```
✅ Using f-strings (modern & readable):
```
print(f"My name is {name} and I am {age} years old.")
```
________________________________________
🔹 3. Type Conversion in Python
Used to convert data from one type to another.
✅ Common Functions:

|Function	|Converts To|
|-----------|-----------|
|int()	|Integer|
|float()	|Float|
|str()	|String|
|bool()	|Boolean|
________________________________________
🔹 4. Examples of Type Conversion
🧪 Convert string input to integer:
```
age = input("Enter your age: ")
age = int(age)  # now it's an integer
print(f"Next year you’ll be {age + 1}")
```
🧪 Float to int:
```
num = 3.99
num_int = int(num)
print(num_int)  # Output: 3
```
🧪 Int to float:
```
x = 5
print(float(x))  # Output: 5.0
```
🧪 String to float:
```
rate = float(input("Enter interest rate: "))
print(rate * 2)
```
________________________________________
✅ Bonus: Check Type
```
x = "123"
print(type(x))  # Output: <class 'str'>

y = int(x)
print(type(y))  # Output: <class 'int'>
```
________________________________________
🧠 Mini Practice
```
name = input("Enter your name: ")
age = int(input("Enter your age: "))
print(f"{name}, you were born in {2025 - age}")
```

### Operators
Operators are symbols or words used to perform operations on variables and values.
________________________________________
✅ Categories of Operators
|Type	|Used |For|
|-------|-----|---|
|Arithmetic Operators	|Basic |math|
|Assignment Operators	|Assigning |values|
|Comparison Operators	|Comparing |values|
|Logical Operators	|Combining |conditions|
|Identity Operators	|Object |identity|
|Membership Operators	|Membership |testing|
|Bitwise Operators	|Binary |operations|
________________________________________
### 🔹 1. Arithmetic Operators
Used for mathematical operations.
|Operator	|Description	|Example|	Result|
|-----------|---------------|-----|----|
|+	|Addition	|5 + 3	| 8|
|-	|Subtraction	|5 - 3	| 2|
|*	|Multiplication	|5 * 3 |	15|
|/	|Division	|5 / 2 |	2.5|
|//	|Floor Division	|5 // 2 | 2|
|%	|Modulus (remainder)	|5 % 2 | 1|
|**	|Exponentiation	|2 ** 3 | 8|
________________________________________
### 🔹 2. Assignment Operators
Used to assign values to variables.
|Operator	|Example	|Same As|
|-----------|-----------|-------|
|=	|x = 5	|Assign 5 to x|
|+=	|x += 3	|x = x + 3|
|-=	|x -= 2	|x = x - 2|
|*=	|x *= 3	|x = x * 3|
|/=	|x /= 2	|x = x / 2|
|//=	|x //= 2	|x = x // 2|
|%=	|x %= 2	|x = x % 2|
|**=	|x **= 2	|x = x ** 2|
________________________________________
### 🔹 3. Comparison Operators
Used to compare values. Returns True or False.
|Operator	|Description	|Example	|Result|
|----------|----------------|----|-----|
|==	|Equal to	|5 == 5|	True|
|!=	|Not equal to	|5 != 3	|True|
|>	|Greater than	|5 > 3	|True|
|<	|Less than	|3 < 5	|True|
|>=	|Greater or equal	|5 >= 5	|True|
|<=	|Less or equal	|5 <= 6	|True|
________________________________________
### 🔹 4. Logical Operators
Used to combine conditional statements.
|Operator	|Description	|Example|	Result|
|-----------|-------------|-----|------|
|and	|True if both are True|	True and False|False|
|or	|True if at least one is True	|True or False | True|
|not	|Reverses the result	|not True | False
________________________________________
### 🔹 5. Identity Operators
Used to compare memory locations (not just values).
|Operator	|Description	|Example	|Result|
|--------------|----------|----|----|
|is	True |if both refer to same object	|a is b | True/False|
|is not	True |if not the same object	|a is not b	| True/False|
🧪 Example:
```
a = [1, 2]
b = a
print(a is b)        # True (same memory)
print(a == b)        # True (same value)

c = [1, 2]
print(a is c)        # False
print(a == c)        # True
```
________________________________________
### 🔹 6. Membership Operators
Used to test whether a value is in a sequence.
|Operator	|Description	|Example	|Result|
|-----------|---------------|----|----|
|in	|True if value exists	|"a" in "cat" |	True|
|not in	|True if value doesn’t	|3 not in [1, 2] | True|
________________________________________
### 🔹 7. Bitwise Operators (Advanced)
Used for binary operations on integers.
|Operator	|Description	|Example|	Result|
|------------|------------|-----------|-----|
|&	|AND	|5 & 3|1
|`	|`	|OR	|`5|
|^	|XOR	|5 ^ 3	|6|
|~	|NOT	|~5	|-6|
|<<	|Left Shift	|5 << 1|	10|
|>>	|Right Shift	|5 >> 1	|2|
________________________________________
🧠 Practice Examples:
```
# Arithmetic
a, b = 10, 3
print(a + b, a % b, a ** b)

# Comparison
print(a > b, a == 10)

# Logical
print((a > 5) and (b < 5))

# Identity
x = [1, 2]
y = [1, 2]
print(x is y, x == y)

# Membership
print("e" in "hello", 2 in [1, 2, 3])
```
________________________________________
Control Flow Statements
Control flow statements allow you to control the execution of your Python code based on conditions and loops.
________________________________________
## 1. Conditional Statements
🔹 if, elif, and else
These statements are used to make decisions in Python.
✅ Syntax:
```
if condition:
    # block of code
elif another_condition:
    # block of code
else:
    # block of code
```
✅ Example:
```
age = 18

if age >= 18:
    print("You are eligible to vote.")
elif age > 0:
    print("You are too young to vote.")
else:
    print("Invalid age")
```

### 🔸 Nested if:
```
num = 10
if num > 0:
    if num % 2 == 0:
        print("Positive Even")
    else:
        print("Positive Odd")
```
________________________________________
## 2. Loops in Python
### 🔹 for Loop
Used to iterate over a sequence (list, string, range, etc.)
✅ Example 1: Iterating a list
```
fruits = ['apple', 'banana', 'cherry']
for fruit in fruits:
    print(fruit)
```
✅ Example 2: Using range()
```
for i in range(1, 6):
    print(i)
```
### 🔹 while Loop
Runs as long as the condition is True.
✅ Example:
```
count = 0
while count < 5:
    print("Count:", count)
    count += 1
```
________________________________________
## 🔁 3. Loop Control Statements
These help manage flow inside loops.
### 🔸 break: Exit the loop early
```
for i in range(10):
    if i == 5:
        break
    print(i)
```
### 🔸 continue: Skip the current iteration
```
for i in range(5):
    if i == 2:
        continue
    print(i)
```
### 🔸 pass: Placeholder (does nothing)
```
for i in range(3):
    pass  # used when code is not yet written
```
________________________________________
## 🔂 4. else with Loops
You can use an else block with loops. It runs only if the loop doesn't break.
✅ Example:
```
for i in range(5):
    print(i)
else:
    print("Loop finished normally.")
```
✅ Example with break:
```
for i in range(5):
    if i == 3:
        break
    print(i)
else:
    print("Won’t print because loop was broken.")
```
________________________________________
## 🧠 Mini Project: Even/Odd Counter
```
nums = [1, 4, 7, 8, 10, 13]
even = 0
odd = 0

for num in nums:
    if num % 2 == 0:
        even += 1
    else:
        odd += 1

print(f"Even numbers: {even}")
print(f"Odd numbers: {odd}")
```
________________________________________
### 📌 Summary Table
|Statement	|Purpose|
|----------|----------|
|if / elif / else	|Decision making|
|for	|Loop through iterable|
|while	|Repeat until condition is false|
|break	|Exit loop early|
|continue	|Skip current iteration|
|pass	|Do nothing (placeholder)|
|else (with loop)	|Run if loop wasn’t broken|

## Python Tutorial: Data Structures in Python (with Key Methods)
📘 What are Data Structures?
Data structures are ways to store and organize data so it can be used efficiently.
Python’s Built-in Data Structures:
1.	List
2.	Tuple
3.	Set
4.	Dictionary
5.	String (optional, sometimes treated as a data structure)
________________________________________
### 🔹 1. List
A list is an ordered, mutable collection.

✅ Create a list:
```
fruits = ['apple', 'banana', 'cherry']
```
✅ Key Methods:

|Method	|Description|
|--------|------|
|append()	|Add item to end|
|insert()	|Insert at a position|
|pop()	|Remove and return item|
|remove()	|Remove specific item|
|sort()	|Sort the list|
|reverse()	|Reverse the list|
|index()	|Find index of an item|
|count()	|Count occurrences|
### 🧪 Example:
```
fruits.append("mango")
fruits.insert(1, "orange")
print(fruits.pop())
print(fruits.index("banana"))
```
________________________________________
### 🔹 2. Tuple
A tuple is an ordered, immutable collection.
✅ Create a tuple:
```
colors = ('red', 'green', 'blue')
```
✅ Key Methods:

|Method	|Description|
|--------|----------|
|count()	|Count occurrences of value|
|index()	|Return first index of value|
### 🧪 Example:
```
print(colors.count("red"))
print(colors.index("blue"))
```
## 🔹 3. Set
A set is an unordered, mutable, no-duplicates collection.

✅ Create a set:
```
nums = {1, 2, 3, 4}
```
✅ Key Methods:

|Method	|Description|
|---------|--------|
|add()	|Add an element|
|update()	|Add multiple elements|
|remove()	|Remove element (error if not found)|
|discard()	|Remove if present|
|clear()	|Remove all elements|
|union()	|Return union of sets|
|intersection()	|Return common elements|
|difference()	|Return difference|
### 🧪 Example:
```
nums.add(5)
nums.update([6, 7])
nums.remove(2)
nums2 = {5, 6, 8}
print(nums.union(nums2))
```
________________________________________
## 🔹 4. Dictionary
A dictionary is an unordered collection of key-value pairs.

✅ Create a dict:
```
student = {
    "name": "Alice",
    "age": 21,
    "course": "Python"
}
```
✅ Key Methods:

|Method	|Description|
|-------|----------|
|get()	|Get value for key|
|keys()	|All keys|
|values()	|All values|
|items()	|All key-value pairs|
|update()	|Update with another dict|
|pop()	|Remove and return value by key|
|clear()	|Remove all items|
### 🧪 Example:
```
print(student.get("name"))
student.update({"age": 22})
print(student.keys())
student.pop("course")
```
## 🔹 5. String (as a bonus)
Strings are immutable sequences of characters.

✅ Create a string:
```
text = "hello python"
```
✅ Key Methods:

|Method	|Description|
|-------|--------|
|upper()	|Convert to uppercase|
|lower()	|Convert to lowercase|
|split()	|Split into list|
|replace()	|Replace text|
|find()	|Find index of substring|
|strip()	|Remove leading/trailing spaces|
### 🧪 Example:
```
print(text.upper())
print(text.replace("python", "world"))
print(text.split())
```
## 🧠 Mini Practice
```
# List
shopping = ["milk", "bread"]
shopping.append("eggs")
shopping.remove("milk")

# Tuple
coords = (10, 20)
print("X:", coords[0])

# Set
unique_nums = set([1, 2, 2, 3])
print(unique_nums)

# Dict
book = {"title": "Python", "pages": 300}
print(book["title"])
```
________________________________________
|Structure	|Ordered	|Mutable	|Duplicate Allowed	|Example Type|
|-----------|--------|---------|-------|-------|
|List	|✅	|✅	|✅	|[]|
|Tuple	|✅	|❌	|✅	|()|
|Set	|❌	|✅	|❌	|{}|
|Dictionary	|❌	|✅	|❌ |(on keys)	{key: val}|

## Python OOPs Tutorial – Beginner to Intermediate

### 🔷 What is OOP?

Object-Oriented Programming (OOP) is a programming paradigm that models real-world entities as objects, with attributes (data) and behaviors (methods).
________________________________________
### 4 Core Pillars of OOP:

|Pillar	|Description|
|-------|----------|
|Encapsulation	|Binding data and methods in a class|
|Abstraction	|Hiding internal details, showing only essentials|
|Inheritance	|Reusing code from parent class|
|Polymorphism	|Same method name behaves differently in classes|
### ✅ 1. Class & Object
🔹 Class: Blueprint for creating objects
🔹 Object: Instance of the class
```
class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

    def start(self):
        print(f"{self.brand} {self.model} is starting...")

# Creating an object
my_car = Car("Toyota", "Camry")
my_car.start()
```
### ✅ 2. Encapsulation
Protects data by restricting access using methods.
```
class BankAccount:
    def __init__(self, owner, balance):
        self.owner = owner
        self.__balance = balance  # private variable

    def deposit(self, amount):
        self.__balance += amount

    def get_balance(self):
        return self.__balance

acc = BankAccount("Alice", 1000)
acc.deposit(500)
print(acc.get_balance())  # 1500
```
### ✅ 3. Abstraction
Hides complex internal logic and shows only the interface.
```
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def sound(self):
        pass

class Dog(Animal):
    def sound(self):
        return "Bark"

d = Dog()
print(d.sound())
```
### ✅ 4. Inheritance
One class inherits properties from another.
```
class Vehicle:
    def __init__(self, brand):
        self.brand = brand

    def start(self):
        print(f"{self.brand} is ready to go!")

class Bike(Vehicle):
    def ring_bell(self):
        print("Ring Ring!")

b = Bike("Hero")
b.start()
b.ring_bell()
```
### ✅ 5. Polymorphism
Same function name behaves differently.
🔹 With Inheritance
```
class Bird:
    def sound(self):
        print("Some generic sound")

class Parrot(Bird):
    def sound(self):
        print("Squawk")

class Crow(Bird):
    def sound(self):
        print("Caw")

for bird in (Parrot(), Crow()):
    bird.sound()
🔹 Operator Overloading
class Book:
    def __init__(self, pages):
        self.pages = pages

    def __add__(self, other):
        return self.pages + other.pages

b1 = Book(100)
b2 = Book(200)
print(b1 + b2)  # 300
```
________________________________________
### 🧠 Important OOP Concepts Quick View
|Concept|Syntax |Feature|
|------|--------|--------|
|Constructor	|__init__() |method|
|Access Modifiers|	self.__private|
|Abstraction	|from abc import ABC,Inheritance|	class B(A)|
|Polymorphism	|Method |Overriding/Overloading|
## 🚀 Mini Project: Student Management System
We'll create a small project that allows:

1.	Adding students
2.	Viewing student details
3.	Calculating average marks
```
class Student:
    def __init__(self, name, roll):
        self.name = name
        self.roll = roll
        self.marks = []

    def add_mark(self, mark):
        self.marks.append(mark)

    def get_average(self):
        if self.marks:
            return sum(self.marks) / len(self.marks)
        return 0

    def display_info(self):
        print(f"Name: {self.name}")
        print(f"Roll No: {self.roll}")
        print(f"Marks: {self.marks}")
        print(f"Average: {self.get_average():.2f}")


# Driver code
students = []

while True:
    print("\n1. Add Student\n2. Show Students\n3. Exit")
    choice = input("Enter choice: ")

    if choice == "1":
        name = input("Enter name: ")
        roll = input("Enter roll no: ")
        s = Student(name, roll)
        for i in range(3):
            mark = int(input(f"Enter mark {i+1}: "))
            s.add_mark(mark)
        students.append(s)

    elif choice == "2":
        for s in students:
            s.display_info()

    elif choice == "3":
        break

    else:
        print("Invalid choice")

```