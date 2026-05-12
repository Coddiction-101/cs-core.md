# 💻 COMPUTER SCIENCE FUNDAMENTALS - Complete Beginner to Advanced Guide

**What is Computer Science?**
CS = Study of computation, problem-solving, and how computers work. It's about THINKING and LOGIC, not just using computers.

---

## 📚 Table of Contents

1. [Part 1: Programming Basics](#part-1-programming-basics)
2. [Part 2: Data Types & Variables](#part-2-data-types--variables)
3. [Part 3: Control Flow](#part-3-control-flow)
4. [Part 4: Functions & Modular Code](#part-4-functions--modular-code)
5. [Part 5: Data Structures](#part-5-data-structures)
6. [Part 6: Algorithms & Problem Solving](#part-6-algorithms--problem-solving)
7. [Part 7: Complexity Analysis](#part-7-complexity-analysis)
8. [Part 8: Object-Oriented Programming](#part-8-object-oriented-programming)
9. [Part 9: Functional Programming](#part-9-functional-programming)
10. [Part 10: Databases & SQL](#part-10-databases--sql)

---

# PART 1: PROGRAMMING BASICS

## 1.1 What is Programming?

**In Simple Terms:** Giving step-by-step instructions to computers to solve problems.

```
Example: Making a Sandwich

Human understands: "Make a sandwich"

Computer needs every detail:
1. Open the cabinet
2. Take out bread
3. Count out 2 slices
4. Place on counter
5. Get butter from fridge
6. Open butter container
7. Take knife
8. Spread butter on first slice
... (50+ more steps)

Computer doesn't understand shortcuts!
It needs EVERY instruction explicit.
```

## 1.2 Programming Languages

**What is a Programming Language?**

Think of it like speaking to the computer in its language.

```
You speak English → Someone translates → Computer
(Understandable)     (Programming)      (Executable)

Different languages, same logic:
Python:    print("Hello")
C:         printf("Hello");
Java:      System.out.println("Hello");
JavaScript: console.log("Hello");

All do same thing, different syntax (grammar rules)
```

### **Popular Programming Languages**

```
Python
├─ Easiest to learn
├─ Great for beginners
├─ Used in: Data science, AI, web, scripting
├─ Syntax: Very simple, looks like English
└─ Best for: Starting your journey

JavaScript
├─ Web development (browser)
├─ Makes websites interactive
├─ Essential if you want web developer
└─ Learning curve: Medium

Java
├─ Object-oriented
├─ "Write once, run anywhere"
├─ Used in: Large companies, Android
└─ Learning curve: Steep

C
├─ Low-level programming
├─ Very fast
├─ Understanding memory, pointers
└─ Learning curve: Very steep

C++
├─ Extension of C
├─ Game development, graphics
├─ Very powerful, very complex
└─ Learning curve: Very steep

Go
├─ Simple, powerful
├─ Great for concurrent programs
├─ Used by: Google, cloud systems
└─ Learning curve: Easy-Medium
```

## 1.3 Why Learn Computer Science?

```
1. Problem-solving skills
   - Break complex problems into small parts
   - Think logically
   - Transfer to real life

2. High salary jobs
   - Software engineer: $80,000 - $300,000+
   - Data scientist: $100,000 - $250,000+
   - Tech is rewarding career

3. Create anything
   - Apps, games, websites
   - AI systems
   - Robotics
   - Your imagination is the limit

4. Automation
   - Computers do boring work
   - You focus on creative/thinking
   - Increase productivity

5. Understanding modern world
   - How technology works
   - Why privacy matters
   - Critical thinking about tech
```

---

# PART 2: DATA TYPES & VARIABLES

## 2.1 What is a Variable?

**In Simple Terms:** A named container that holds data/values.

```
Think of it like:
- A box with a label
- A sticky note with name and value
- A storage location in computer memory

Real example:
name = "Alice"
age = 25
height = 5.9

"name" is the label
"Alice" is what's inside
We can use "name" to refer to "Alice" later
```

## 2.2 Basic Data Types

### **String (Text)**

```
What it is: Text, characters, words, sentences

Examples:
name = "Alice"
city = "New York"
message = "Hello, World!"
empty = ""

Common operations:
name = "Alice"
print(name)              # Alice
print(name.upper())      # ALICE
print(name.lower())      # alice
print(len(name))         # 5
print(name[0])           # A (first character)
print(name.replace("A", "B"))  # Blice

Combining strings:
first = "John"
last = "Doe"
full = first + " " + last  # "John Doe"
```

### **Integer (Whole Numbers)**

```
What it is: Numbers without decimal point

Examples:
age = 25
year = 2024
temperature = -5
balance = 1000

Common operations:
a = 10
b = 3
print(a + b)    # 13 (addition)
print(a - b)    # 7 (subtraction)
print(a * b)    # 30 (multiplication)
print(a / b)    # 3.333... (division)
print(a // b)   # 3 (integer division - drops decimal)
print(a % b)    # 1 (remainder/modulo)
print(a ** b)   # 1000 (exponent: 10^3)
```

### **Float (Decimal Numbers)**

```
What it is: Numbers with decimal point

Examples:
price = 19.99
height = 5.9
pi = 3.14159
temperature = 98.6

Operations same as integer:
a = 10.5
b = 3.2
print(a + b)    # 13.7
print(a * b)    # 33.6
```

### **Boolean (True/False)**

```
What it is: Only two values possible

Examples:
is_student = True
is_raining = False
has_license = True

Used for decision making:
temperature = 35
is_hot = temperature > 30  # True
print(is_hot)              # True
```

### **None (Nothing)**

```
What it is: Represents absence of value

Example:
result = None  # No value yet

Used when:
- Variable not initialized
- Function returns no value
- Intentional "empty" state
```

## 2.3 Getting User Input

```
How to get information from user:

Python:
name = input("What is your name? ")
# User types: Alice
# name now equals "Alice"

age_input = input("How old are you? ")
age = int(age_input)  # Convert text to number
# age now equals the number, not text

height = float(input("Your height: "))  # Convert to decimal
```

## 2.4 Printing Output

```
Displaying information to user:

Python:
print("Hello")                      # Hello
print(name)                         # Alice
print("My name is", name)          # My name is Alice
print(f"Hi, I'm {name}")           # Hi, I'm Alice (f-string)
print("Age: " + str(age))          # Age: 25 (converting number to text)
```

---

# PART 3: CONTROL FLOW

## 3.1 If Statements (Making Decisions)

**Concept:** Execute code only if condition is true.

```
Logic:

If (condition is TRUE) → Do this
Otherwise → Do that

Simple Example:
```

```python
age = 20

if age >= 18:
    print("You can vote")
else:
    print("You're too young")

# Output: You can vote
```

```
More Complex Example:
```

```python
score = 85

if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
else:
    print("Grade: F")

# Output: Grade: B
```

**Comparison Operators:**
```
==    Equal to
!=    Not equal to
>     Greater than
<     Less than
>=    Greater than or equal
<=    Less than or equal
```

**Logical Operators:**
```
and   Both conditions must be true
or    Either condition can be true
not   Opposite of condition

Example:
age = 25
has_license = True

if age >= 18 and has_license:
    print("Can drive")
# Output: Can drive

if age < 21 or not has_license:
    print("Cannot drink")
# Output: Cannot drink (has_license is true, but or needs only one)
```

## 3.2 Loops (Repeating Code)

**Concept:** Repeat code multiple times.

### **While Loop**

```
Repeat while condition is true:

counter = 0
while counter < 5:
    print(counter)
    counter = counter + 1

Output:
0
1
2
3
4
```

**Real Example:**
```python
password = ""
correct_password = "secret123"

while password != correct_password:
    password = input("Enter password: ")
    if password == correct_password:
        print("Access granted!")
    else:
        print("Wrong password, try again")
```

### **For Loop**

```
Repeat a certain number of times:

for i in range(5):
    print(i)

Output:
0
1
2
3
4

range(5) means 0, 1, 2, 3, 4 (stops before 5)
```

**For Loop with List:**
```python
fruits = ["apple", "banana", "orange"]

for fruit in fruits:
    print(fruit)

Output:
apple
banana
orange
```

**For Loop with Index:**
```python
fruits = ["apple", "banana", "orange"]

for i in range(len(fruits)):
    print(f"{i}: {fruits[i]}")

Output:
0: apple
1: banana
2: orange
```

### **Loop Control**

```python
# Break (exit loop completely)
for i in range(10):
    if i == 5:
        break  # Stop loop
    print(i)
# Output: 0 1 2 3 4

# Continue (skip to next iteration)
for i in range(5):
    if i == 2:
        continue  # Skip this iteration
    print(i)
# Output: 0 1 3 4

# Break and Continue together
for i in range(10):
    if i == 2:
        continue  # Skip 2
    if i == 7:
        break  # Stop at 7
    print(i)
# Output: 0 1 3 4 5 6
```

---

# PART 4: FUNCTIONS & MODULAR CODE

## 4.1 What is a Function?

**In Simple Terms:** Reusable block of code that does something specific.

```
Without functions (Bad):
# Calculate area for square 1
side1 = 5
area1 = side1 * side1
print(f"Area: {area1}")

# Calculate area for square 2
side2 = 10
area2 = side2 * side2
print(f"Area: {area2}")

# Calculate area for square 3
side3 = 15
area3 = side3 * side3
print(f"Area: {area3}")

(Lots of repetition!)


With functions (Good):
def calculate_square_area(side):
    return side * side

print(calculate_square_area(5))   # 25
print(calculate_square_area(10))  # 100
print(calculate_square_area(15))  # 225

(Clean, reusable!)
```

## 4.2 Creating Functions

```python
def function_name(parameter1, parameter2):
    """Docstring: explanation of function"""
    # Code here
    return result

Example:
def add(a, b):
    """Add two numbers"""
    result = a + b
    return result

print(add(5, 3))  # 8
```

## 4.3 Function Parameters

```python
# No parameters
def greet():
    print("Hello!")

greet()  # Hello!

# One parameter
def greet_person(name):
    print(f"Hello, {name}!")

greet_person("Alice")  # Hello, Alice!

# Multiple parameters
def add(a, b):
    return a + b

print(add(5, 3))  # 8

# Default parameters
def greet_person(name, greeting="Hello"):
    print(f"{greeting}, {name}!")

greet_person("Alice")                    # Hello, Alice!
greet_person("Bob", "Hi")               # Hi, Bob!
greet_person("Carol", "Howdy")          # Howdy, Carol!

# Variable number of arguments
def sum_all(*numbers):
    total = 0
    for num in numbers:
        total = total + num
    return total

print(sum_all(1, 2, 3))          # 6
print(sum_all(1, 2, 3, 4, 5))    # 15
```

## 4.4 Return Values

```python
# No return
def print_twice(text):
    print(text)
    print(text)

print_twice("Hi")  # Prints Hi twice, doesn't return anything

# Return single value
def square(n):
    return n * n

result = square(5)
print(result)  # 25

# Return multiple values
def divide_and_remainder(a, b):
    quotient = a // b
    remainder = a % b
    return quotient, remainder

q, r = divide_and_remainder(10, 3)
print(q)  # 3
print(r)  # 1
```

## 4.5 Scope (Where Variables Live)

```python
global_var = "I'm global"  # Accessible everywhere

def my_function():
    local_var = "I'm local"  # Only accessible in this function
    print(global_var)   # Works (can access global)
    print(local_var)    # Works

my_function()  # I'm global, I'm local
print(local_var)  # ERROR! Not accessible outside function
```

---

# PART 5: DATA STRUCTURES

## 5.1 Lists (Collections of Items)

**What it is:** Ordered collection of items that can change.

```python
# Create list
numbers = [1, 2, 3, 4, 5]
fruits = ["apple", "banana", "orange"]
mixed = [1, "hello", 3.14, True]

# Access items (indexing starts at 0)
numbers[0]      # 1 (first item)
numbers[2]      # 3 (third item)
numbers[-1]     # 5 (last item)
numbers[-2]     # 4 (second to last)

# Modify items
fruits[0] = "grape"  # Change first item
# ["grape", "banana", "orange"]

# Add items
fruits.append("kiwi")
# ["grape", "banana", "orange", "kiwi"]

fruits.insert(1, "mango")  # Insert at position 1
# ["grape", "mango", "banana", "orange", "kiwi"]

# Remove items
fruits.remove("banana")  # Remove by value
# ["grape", "mango", "orange", "kiwi"]

fruits.pop()  # Remove last item
# ["grape", "mango", "orange"]

# List length
len(fruits)  # 3

# Check if item exists
"grape" in fruits  # True
"banana" in fruits  # False

# List operations
list1 = [1, 2, 3]
list2 = [4, 5, 6]
combined = list1 + list2  # [1, 2, 3, 4, 5, 6]

# Loop through list
for fruit in fruits:
    print(fruit)
# Output: grape, mango, orange
```

## 5.2 Tuples (Immutable Lists)

**What it is:** Like a list, but can't be changed after creation.

```python
# Create tuple
coordinates = (10, 20)
colors = ("red", "green", "blue")

# Access items (same as list)
colors[0]  # "red"
colors[-1]  # "blue"

# Check length
len(colors)  # 3

# Check if exists
"red" in colors  # True

# CANNOT modify
colors[0] = "yellow"  # ERROR!
colors.append("yellow")  # ERROR!

# Use when you want to protect data
def get_coordinates():
    return (10, 20)  # Can't be accidentally modified
```

## 5.3 Dictionaries (Key-Value Pairs)

**What it is:** Data stored by key-value pairs, like a real dictionary.

```python
# Create dictionary
person = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}

# Access by key
person["name"]  # "Alice"
person["age"]   # 25

# Add new key-value
person["job"] = "Engineer"
# {"name": "Alice", "age": 25, "city": "New York", "job": "Engineer"}

# Modify value
person["age"] = 26

# Remove key-value
del person["city"]

# Check if key exists
"name" in person  # True
"email" in person  # False

# Get all keys
keys = person.keys()  # ["name", "age", "job"]

# Get all values
values = person.values()  # ["Alice", 26, "Engineer"]

# Get all items
items = person.items()  # [("name", "Alice"), ("age", 26), ...]

# Loop through dictionary
for key, value in person.items():
    print(f"{key}: {value}")
# Output:
# name: Alice
# age: 26
# job: Engineer

# Real use case: Student grades
grades = {
    "Alice": 95,
    "Bob": 87,
    "Carol": 92
}

print(grades["Alice"])  # 95
```

## 5.4 Sets (Unique Items)

**What it is:** Collection of unique items (no duplicates).

```python
# Create set
colors = {"red", "green", "blue"}
numbers = {1, 2, 3, 3, 2}  # Duplicates removed

print(numbers)  # {1, 2, 3}

# Add item
colors.add("yellow")

# Remove item
colors.remove("red")

# Check if exists
"blue" in colors  # True

# Set operations
set1 = {1, 2, 3}
set2 = {3, 4, 5}

union = set1 | set2  # {1, 2, 3, 4, 5}
intersection = set1 & set2  # {3}
difference = set1 - set2  # {1, 2}

# Use case: Remove duplicates
my_list = [1, 2, 2, 3, 3, 3, 4]
unique = set(my_list)  # {1, 2, 3, 4}
```

---

# PART 6: ALGORITHMS & PROBLEM SOLVING

## 6.1 What is an Algorithm?

**In Simple Terms:** Step-by-step procedure to solve a problem.

```
Not specific to computers!

Cooking algorithm (recipe):
1. Gather ingredients
2. Mix flour and eggs
3. Heat pan
4. Pour mixture
5. Cook until done
6. Serve

Computer algorithm:
1. Get list of numbers
2. Compare first two
3. Swap if first is larger
4. Move to next pair
5. Repeat until sorted
```

## 6.2 Sorting Algorithms

### **Bubble Sort (Simple but Slow)**

```python
def bubble_sort(arr):
    n = len(arr)
    # Outer loop: number of passes
    for i in range(n):
        # Inner loop: compare adjacent items
        for j in range(0, n - i - 1):
            # Swap if first is larger
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]
    return arr

numbers = [64, 34, 25, 12, 22, 11, 90]
print(bubble_sort(numbers))
# Output: [11, 12, 22, 25, 34, 64, 90]

Visualization:
Pass 1: [34, 25, 12, 22, 11, 64, 90] (64 and 90 in place)
Pass 2: [25, 12, 22, 11, 34, 64, 90] (34 in place)
...continues...
Final:  [11, 12, 22, 25, 34, 64, 90]
```

### **Selection Sort**

```python
def selection_sort(arr):
    n = len(arr)
    for i in range(n):
        # Find minimum in remaining array
        min_idx = i
        for j in range(i + 1, n):
            if arr[j] < arr[min_idx]:
                min_idx = j
        # Swap minimum to beginning
        arr[i], arr[min_idx] = arr[min_idx], arr[i]
    return arr
```

### **Merge Sort (Fast)**

```python
def merge_sort(arr):
    # Base case: already sorted
    if len(arr) <= 1:
        return arr
    
    # Divide in half
    mid = len(arr) // 2
    left = merge_sort(arr[:mid])
    right = merge_sort(arr[mid:])
    
    # Merge back together
    return merge(left, right)

def merge(left, right):
    result = []
    i = j = 0
    
    while i < len(left) and j < len(right):
        if left[i] <= right[j]:
            result.append(left[i])
            i += 1
        else:
            result.append(right[j])
            j += 1
    
    result.extend(left[i:])
    result.extend(right[j:])
    return result

numbers = [64, 34, 25, 12, 22, 11, 90]
print(merge_sort(numbers))
# Output: [11, 12, 22, 25, 34, 64, 90]
```

## 6.3 Searching Algorithms

### **Linear Search**

```python
def linear_search(arr, target):
    for i in range(len(arr)):
        if arr[i] == target:
            return i  # Found at position i
    return -1  # Not found

numbers = [10, 20, 30, 40, 50]
print(linear_search(numbers, 30))  # 2
print(linear_search(numbers, 60))  # -1
```

### **Binary Search (Fast, requires sorted array)**

```python
def binary_search(arr, target):
    left = 0
    right = len(arr) - 1
    
    while left <= right:
        mid = (left + right) // 2
        
        if arr[mid] == target:
            return mid  # Found!
        elif arr[mid] < target:
            left = mid + 1  # Search right half
        else:
            right = mid - 1  # Search left half
    
    return -1  # Not found

numbers = [10, 20, 30, 40, 50]
print(binary_search(numbers, 30))  # 2
print(binary_search(numbers, 60))  # -1

Visual example:
Array: [10, 20, 30, 40, 50]
Looking for: 30

Step 1: Check middle (30) → Found! Return 2
```

## 6.4 Recursion (Function Calls Itself)

**What it is:** A function that calls itself to solve smaller version of problem.

```python
# Factorial example
def factorial(n):
    # Base case: when to stop
    if n <= 1:
        return 1
    
    # Recursive case: call itself
    return n * factorial(n - 1)

factorial(5)
= 5 * factorial(4)
= 5 * 4 * factorial(3)
= 5 * 4 * 3 * factorial(2)
= 5 * 4 * 3 * 2 * factorial(1)
= 5 * 4 * 3 * 2 * 1
= 120

print(factorial(5))  # 120
```

**Key Rules:**
```
1. Base case: When to STOP (prevent infinite loop)
2. Recursive case: Call function with smaller problem
3. Progress toward base case: Each call gets closer
```

---

# PART 7: COMPLEXITY ANALYSIS

## 7.1 What is Complexity?

**In Simple Terms:** How long does an algorithm take (Time) and how much memory it uses (Space)?

## 7.2 Big O Notation

**What it measures:** How algorithm performance scales with input size.

```
O(1)        Constant: Same time regardless of size
O(log n)    Logarithmic: Half the remaining each time
O(n)        Linear: Time grows with size
O(n log n)  Linearithmic: Between linear and quadratic
O(n²)       Quadratic: Time grows with size squared
O(2ⁿ)       Exponential: Doubles with each addition
O(n!)       Factorial: Grows extremely fast
```

### **Visual Comparison (1 million items)**

```
O(1)        1 nanosecond
O(log n)    20 nanoseconds
O(n)        1 second
O(n log n)  20 seconds
O(n²)       12 days
O(2ⁿ)       Impossible (universe would end)
```

### **Real Examples**

```python
# O(1) - Constant time
def get_first(arr):
    return arr[0]  # Always 1 step

# O(n) - Linear time
def find_max(arr):
    max_val = arr[0]
    for item in arr:  # Loop through all items
        if item > max_val:
            max_val = item
    return max_val

# O(n²) - Quadratic time
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):           # Loop n times
        for j in range(n - i - 1):  # Loop n times again
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]
    # Nested loops = n * n = n²

# O(log n) - Logarithmic time
def binary_search(arr, target):
    left, right = 0, len(arr) - 1
    while left <= right:  # Eliminates half each time
        mid = (left + right) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return -1
```

## 7.3 Choosing Algorithms

```
Problem: Sort 1 million numbers

Bubble Sort O(n²):     12 days
Merge Sort O(n log n): 20 seconds

Choice: Merge Sort (600x faster!)

This is why algorithm choice matters!
```

---

# PART 8: OBJECT-ORIENTED PROGRAMMING

## 8.1 What is OOP?

**In Simple Terms:** Organize code by creating "objects" that represent real things.

```
Without OOP (Procedural):
name = "Alice"
age = 25
salary = 50000

print(f"{name} is {age} years old")
# Hard to organize, lots of separate variables

With OOP (Object-Oriented):
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def greet(self):
        print(f"Hi, I'm {self.name}")

alice = Person("Alice", 25)
alice.greet()  # Hi, I'm Alice
# Much more organized!
```

## 8.2 Classes and Objects

**Class:** Blueprint or template
**Object:** Actual instance of the blueprint

```python
# Class (blueprint)
class Dog:
    def __init__(self, name, breed):
        self.name = name
        self.breed = breed
    
    def bark(self):
        return f"{self.name} says woof!"

# Objects (instances)
dog1 = Dog("Buddy", "Golden Retriever")
dog2 = Dog("Max", "German Shepherd")

print(dog1.bark())  # Buddy says woof!
print(dog2.bark())  # Max says woof!
```

## 8.3 Inheritance (Extending Classes)

**Concept:** Child class inherits from parent class.

```python
# Parent class
class Animal:
    def __init__(self, name):
        self.name = name
    
    def make_sound(self):
        pass

# Child class
class Dog(Animal):
    def make_sound(self):
        return f"{self.name} barks"

class Cat(Animal):
    def make_sound(self):
        return f"{self.name} meows"

# Create objects
dog = Dog("Buddy")
cat = Cat("Whiskers")

print(dog.make_sound())  # Buddy barks
print(cat.make_sound())  # Whiskers meows
```

## 8.4 Encapsulation (Data Hiding)

**Concept:** Hide internal details, expose only what's needed.

```python
class BankAccount:
    def __init__(self, owner, balance):
        self.owner = owner
        self.__balance = balance  # Private (double underscore)
    
    def deposit(self, amount):
        if amount > 0:
            self.__balance += amount
            return f"Deposited ${amount}"
    
    def withdraw(self, amount):
        if 0 < amount <= self.__balance:
            self.__balance -= amount
            return f"Withdrew ${amount}"
        return "Insufficient funds"
    
    def get_balance(self):
        return self.__balance

account = BankAccount("Alice", 1000)
print(account.deposit(500))     # Deposited $500
print(account.get_balance())    # 1500
# Can't access __balance directly:
# print(account.__balance)  # ERROR!
```

---

# PART 9: FUNCTIONAL PROGRAMMING

## 9.1 What is Functional Programming?

**In Simple Terms:** Functions as primary building blocks. Data immutable (doesn't change).

```python
# Imperative (telling how)
numbers = [1, 2, 3, 4, 5]
result = []
for num in numbers:
    if num % 2 == 0:
        result.append(num * 2)
# [4, 8]

# Functional (telling what)
numbers = [1, 2, 3, 4, 5]
result = list(map(lambda x: x * 2, filter(lambda x: x % 2 == 0, numbers)))
# [4, 8]
```

## 9.2 Map, Filter, Reduce

### **Map (Transform each item)**

```python
numbers = [1, 2, 3, 4, 5]
doubled = list(map(lambda x: x * 2, numbers))
print(doubled)  # [2, 4, 6, 8, 10]

# More readable:
doubled = [x * 2 for x in numbers]  # List comprehension
```

### **Filter (Keep matching items)**

```python
numbers = [1, 2, 3, 4, 5, 6]
evens = list(filter(lambda x: x % 2 == 0, numbers))
print(evens)  # [2, 4, 6]

# More readable:
evens = [x for x in numbers if x % 2 == 0]
```

### **Reduce (Combine to single value)**

```python
from functools import reduce

numbers = [1, 2, 3, 4, 5]
sum_all = reduce(lambda a, b: a + b, numbers)
print(sum_all)  # 15

# Simpler:
sum_all = sum(numbers)
```

## 9.3 Lambda Functions (Quick Functions)

```python
# Regular function
def add(a, b):
    return a + b

# Lambda function (same thing, shorter)
add = lambda a, b: a + b

print(add(5, 3))  # 8

# Most useful with map/filter:
numbers = [1, 2, 3, 4, 5]
squared = map(lambda x: x ** 2, numbers)
print(list(squared))  # [1, 4, 9, 16, 25]
```

---

# PART 10: DATABASES & SQL

## 10.1 What is a Database?

**In Simple Terms:** Organized storage for data that allows searching, sorting, updating.

```
Without database (Chaos):
students.txt:   Alice, 25, alice@example.com
students.txt:   Bob, 22, bob@example.com
spreadsheet:    Carol, 23, carol@example.com

Hard to search, easy to lose data, inconsistent

With database (Organized):
Table: Students
┌────┬───────┬─────┬──────────────────────┐
│ ID │ Name  │ Age │ Email                │
├────┼───────┼─────┼──────────────────────┤
│ 1  │ Alice │ 25  │ alice@example.com    │
│ 2  │ Bob   │ 22  │ bob@example.com      │
│ 3  │ Carol │ 23  │ carol@example.com    │
└────┴───────┴─────┴──────────────────────┘

Easy to search, organized, consistent
```

## 10.2 Relational Databases

**Concept:** Data in tables, tables can relate to each other.

```
Table 1: Students
┌─────┬───────┐
│ ID  │ Name  │
├─────┼───────┤
│ 1   │ Alice │
│ 2   │ Bob   │
└─────┴───────┘

Table 2: Courses
┌────┬──────────────┬─────────────┐
│ ID │ Course       │ Student_ID  │
├────┼──────────────┼─────────────┤
│ 1  │ Math         │ 1           │
│ 2  │ English      │ 2           │
│ 3  │ Math         │ 2           │
└────┴──────────────┴─────────────┘

Tables relate through Student_ID (Foreign Key)
Alice (ID 1) → Takes Math
Bob (ID 2) → Takes English and Math
```

## 10.3 SQL Basics

**SQL:** Language to talk to databases.

```sql
-- CREATE TABLE (set up structure)
CREATE TABLE students (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    email VARCHAR(100)
);

-- INSERT (add data)
INSERT INTO students (id, name, age, email)
VALUES (1, 'Alice', 25, 'alice@example.com');

-- SELECT (get data)
SELECT * FROM students;
SELECT name, email FROM students;
SELECT * FROM students WHERE age > 20;

-- UPDATE (change data)
UPDATE students
SET age = 26
WHERE name = 'Alice';

-- DELETE (remove data)
DELETE FROM students
WHERE name = 'Bob';
```

## 10.4 Connecting to Databases in Python

```python
import sqlite3

# Connect to database
conn = sqlite3.connect('students.db')
cursor = conn.cursor()

# Create table
cursor.execute('''
    CREATE TABLE students (
        id INTEGER PRIMARY KEY,
        name TEXT,
        age INTEGER
    )
''')

# Insert data
cursor.execute('''
    INSERT INTO students (name, age)
    VALUES (?, ?)
''', ('Alice', 25))

# Get data
cursor.execute('SELECT * FROM students')
for row in cursor.fetchall():
    print(row)

# Save changes
conn.commit()

# Close connection
conn.close()
```

---

## 🎯 Quick Reference

### **Data Type Cheat Sheet**

| Type | Example | Use |
|------|---------|-----|
| String | "Alice" | Text |
| Int | 25 | Whole numbers |
| Float | 5.9 | Decimals |
| Boolean | True | Yes/No |
| List | [1, 2, 3] | Multiple items, changeable |
| Tuple | (1, 2, 3) | Multiple items, fixed |
| Dict | {"name": "Alice"} | Key-value pairs |
| Set | {1, 2, 3} | Unique items |

### **Operator Cheat Sheet**

| Operator | Meaning | Example |
|----------|---------|---------|
| + | Add | 5 + 3 = 8 |
| - | Subtract | 5 - 3 = 2 |
| * | Multiply | 5 * 3 = 15 |
| / | Divide | 5 / 2 = 2.5 |
| // | Integer divide | 5 // 2 = 2 |
| % | Modulo | 5 % 2 = 1 |
| ** | Exponent | 5 ** 2 = 25 |
| == | Equal | 5 == 5 → True |
| != | Not equal | 5 != 3 → True |
| > | Greater | 5 > 3 → True |
| < | Less | 5 < 3 → False |
| >= | Greater/equal | 5 >= 5 → True |
| <= | Less/equal | 5 <= 3 → False |
| and | Both true | True and True → True |
| or | Either true | True or False → True |
| not | Opposite | not True → False |

### **Algorithm Complexity Summary**

| Algorithm | Best | Average | Worst |
|-----------|------|---------|-------|
| Linear Search | O(1) | O(n) | O(n) |
| Binary Search | O(1) | O(log n) | O(log n) |
| Bubble Sort | O(n) | O(n²) | O(n²) |
| Merge Sort | O(n log n) | O(n log n) | O(n log n) |
| Selection Sort | O(n²) | O(n²) | O(n²) |

---

## 🚀 Learning Progression

**Week 1-2: Fundamentals**
- Data types
- Variables
- Operators
- Input/Output

**Week 3-4: Control Flow**
- If statements
- Loops (while, for)
- Break/Continue

**Week 5-6: Functions**
- Creating functions
- Parameters
- Return values
- Scope

**Week 7-8: Data Structures**
- Lists, Tuples
- Dictionaries, Sets
- List operations

**Week 9-10: Algorithms**
- Sorting
- Searching
- Recursion

**Week 11-12: Advanced**
- OOP basics
- Functional programming
- Databases

---

## 📚 Summary

**What You Now Know:**

1. ✓ What programming is and why it matters
2. ✓ Data types and variables
3. ✓ Control flow (if, loops)
4. ✓ Functions and code organization
5. ✓ Data structures (lists, dicts, sets)
6. ✓ Algorithms and problem-solving
7. ✓ Time/space complexity
8. ✓ Object-oriented programming basics
9. ✓ Functional programming concepts
10. ✓ Databases and SQL

**Practice Tips:**

- Write code every day
- Don't just watch tutorials, code along
- Practice problems on LeetCode, HackerRank
- Build small projects
- Debug your own code
- Read other people's code
- Join programming communities

**Next Steps:**

- Pick a language to master (Python is easiest)
- Build projects: Calculator, To-do list, Game
- Learn Web Development (HTML, CSS, JavaScript)
- Explore specialized areas: Data Science, AI, Games
- Contribute to open source

---
