# 🎓 Computer Science & IT Fundamentals: Complete Guide
## From Absolute Beginner to Advanced Professional

**Last Updated:** 2026 | **Difficulty Levels:** Beginner → Intermediate → Advanced

---

## 📚 Table of Contents

1. [Introduction & Roadmap](#introduction--roadmap)
2. [Part 1: Computer Basics](#part-1-computer-basics)
3. [Part 2: Programming Fundamentals](#part-2-programming-fundamentals)
4. [Part 3: Data Structures & Algorithms](#part-3-data-structures--algorithms)
5. [Part 4: Object-Oriented Programming](#part-4-object-oriented-programming)
6. [Part 5: Databases & SQL](#part-5-databases--sql)
7. [Part 6: Web Development](#part-6-web-development)
8. [Part 7: System Design & Architecture](#part-7-system-design--architecture)
9. [Part 8: Operating Systems](#part-8-operating-systems)
10. [Part 9: Computer Networks](#part-9-computer-networks)
11. [Part 10: DevOps & Cloud Computing](#part-10-devops--cloud-computing)
12. [Part 11: Security & Cryptography](#part-11-security--cryptography)
13. [Part 12: Software Engineering Best Practices](#part-12-software-engineering-best-practices)
14. [Part 13: Advanced Topics](#part-13-advanced-topics)
15. [Learning Resources & Tools](#learning-resources--tools)
16. [Interview Preparation Guide](#interview-preparation-guide)

---

## Introduction & Roadmap

### Why This Guide Exists
This comprehensive guide bridges the gap between being a complete beginner and becoming a professional developer ready to tackle complex problems. It covers every essential CS topic with explanations, code examples, and practical insights.

### Learning Path Recommendations

**3 Months (Foundation)**
- Computer Basics → Programming Fundamentals → Data Structures

**6 Months (Core Development)**
- + OOP → Databases → Web Basics

**12 Months (Professional Ready)**
- + System Design → Networks → DevOps → Security

---

# PART 1: COMPUTER BASICS

## 1.1 How Computers Work

### The Fundamental Concept
A computer is an electronic device that processes **data** using **instructions** (programs) to produce **output**.

```
INPUT → PROCESSING → OUTPUT → STORAGE
```

### Binary & Number Systems

#### Binary (Base-2)
- Only uses 0 and 1
- Everything in computers is represented in binary
- 1 bit = smallest unit of information

```
Decimal → Binary
0 → 0
1 → 1
2 → 10
3 → 11
4 → 100
8 → 1000
255 → 11111111 (8 bits)
```

#### Other Number Systems
- **Hexadecimal (Base-16):** 0-9, A-F (used in memory addresses, colors)
- **Octal (Base-8):** 0-7 (less common)

```
Example: #FF5733 (hex color)
FF = Red (255)
57 = Green (87)
33 = Blue (51)
```

### Data Representation

#### Bits and Bytes
```
1 Bit = 0 or 1
1 Byte = 8 bits (0-255)
1 Kilobyte (KB) = 1,024 bytes
1 Megabyte (MB) = 1,024 KB
1 Gigabyte (GB) = 1,024 MB
1 Terabyte (TB) = 1,024 GB
```

#### Character Encoding
- **ASCII:** 7-bit standard (128 characters)
- **Extended ASCII:** 8-bit (256 characters)
- **Unicode:** 16-32 bit (supports all languages)

```
Example ASCII:
'A' = 65
'a' = 97
'0' = 48
' ' (space) = 32
```

### Hardware Components

#### 1. **CPU (Central Processing Unit)**
- "Brain" of the computer
- Executes instructions
- Measured in GHz (cycles per second)
- Multiple cores = parallel processing

#### 2. **RAM (Random Access Memory)**
- Fast, temporary memory
- Volatile (data lost on shutdown)
- Used for active programs and data
- Typical: 8GB, 16GB, 32GB+

#### 3. **Storage**
- **HDD (Hard Disk Drive):** Mechanical, slower, cheaper, larger capacity
- **SSD (Solid State Drive):** No moving parts, faster, more expensive, smaller capacity
- Persistent (data survives shutdown)

#### 4. **Motherboard**
- Central circuit board
- Connects all components

#### 5. **GPU (Graphics Processing Unit)**
- Specialized for parallel processing
- Original: graphics/gaming
- Now: AI, machine learning, scientific computing

#### 6. **Power Supply Unit (PSU)**
- Provides electrical power
- Must match component requirements

### Memory Hierarchy

```
┌─────────────────────────────────────┐
│ CPU Registers (FASTEST, SMALLEST)   │ ~64 bits
├─────────────────────────────────────┤
│ L1 Cache                            │ ~32-64 KB
├─────────────────────────────────────┤
│ L2 Cache                            │ ~256 KB - 512 KB
├─────────────────────────────────────┤
│ L3 Cache                            │ ~8 MB - 16 MB
├─────────────────────────────────────┤
│ RAM (Main Memory)                   │ ~8 GB - 64 GB
├─────────────────────────────────────┤
│ SSD/HDD (SLOWEST, LARGEST)          │ ~256 GB - 2 TB+
└─────────────────────────────────────┘
```

**Speed vs Capacity Trade-off:** Registers are fastest but smallest. Storage is largest but slowest.

## 1.2 Operating Systems (OS)

### What is an OS?
Software that manages hardware resources and provides an interface for programs.

### Main Functions
1. **Process Management:** Run multiple programs
2. **Memory Management:** Allocate RAM efficiently
3. **File System:** Store and organize files
4. **I/O Management:** Handle keyboards, mice, printers
5. **Security:** Protect data and systems

### Popular Operating Systems
- **Windows:** GUI-based, widely used
- **macOS:** Unix-based, for Apple devices
- **Linux:** Open-source, free, server-dominant
- **Android/iOS:** Mobile operating systems

### File Systems
```
C:\ (Windows)                /home (Linux)
├── Program Files            ├── username/
├── Users/                   │   ├── Documents/
│   └── Documents/           │   ├── Downloads/
├── Windows/                 │   └── Pictures/
└── Temp/                    └── etc/
```

---

# PART 2: PROGRAMMING FUNDAMENTALS

## 2.1 What is Programming?

Programming is giving step-by-step instructions to a computer to solve problems.

### Programming Languages Paradigms

#### 1. **Imperative (How-to)**
- Tells computer HOW to do things
- Examples: C, Java, Python, C++

```python
# Imperative: Step by step instructions
sum = 0
for i in range(1, 6):
    sum += i
print(sum)  # Output: 15
```

#### 2. **Declarative (What)**
- Tells computer WHAT you want
- Examples: SQL, HTML, CSS

```sql
-- Declarative: Just say what you want
SELECT name FROM employees WHERE salary > 50000;
```

#### 3. **Functional**
- Functions as primary building blocks
- Immutability, pure functions
- Examples: Lisp, Haskell, Erlang

```python
# Functional approach
result = sum(map(lambda x: x**2, [1, 2, 3]))  # 14
```

#### 4. **Object-Oriented**
- Programs as objects with properties and methods
- Examples: Java, C#, Python

```python
# OOP approach
class Calculator:
    def add(self, a, b):
        return a + b
```

## 2.2 Basic Programming Concepts

### Variables & Data Types

```python
# INTEGERS
age = 25
print(type(age))  # <class 'int'>

# FLOATS (Decimal)
height = 5.9
print(type(height))  # <class 'float'>

# STRINGS (Text)
name = "Alice"
print(type(name))  # <class 'str'>

# BOOLEANS (True/False)
is_student = True
print(type(is_student))  # <class 'bool'>

# LISTS (Ordered, changeable)
numbers = [1, 2, 3, 4, 5]
numbers[0] = 10

# TUPLES (Ordered, unchangeable)
coordinates = (10, 20)
# coordinates[0] = 15  # ERROR!

# DICTIONARIES (Key-Value pairs)
person = {"name": "Bob", "age": 30}
print(person["name"])  # Bob

# SETS (Unique, unordered)
unique_numbers = {1, 2, 3, 3}  # {1, 2, 3}
```

### Operators

```python
# ARITHMETIC
a = 10
b = 3
print(a + b)   # 13
print(a - b)   # 7
print(a * b)   # 30
print(a / b)   # 3.333...
print(a // b)  # 3 (integer division)
print(a % b)   # 1 (modulo/remainder)
print(a ** b)  # 1000 (exponentiation)

# COMPARISON
print(a == b)   # False
print(a != b)   # True
print(a > b)    # True
print(a >= b)   # True

# LOGICAL
print(True and False)  # False
print(True or False)   # True
print(not True)        # False

# ASSIGNMENT
x = 5
x += 2  # x = 7
x -= 1  # x = 6
x *= 2  # x = 12
```

### Control Flow

#### IF Statements
```python
age = 20

if age < 13:
    print("Child")
elif age < 18:
    print("Teenager")
elif age < 65:
    print("Adult")
else:
    print("Senior")
```

#### LOOPS

**While Loop:**
```python
i = 0
while i < 5:
    print(i)
    i += 1
# Output: 0 1 2 3 4
```

**For Loop:**
```python
# Iterating over a sequence
for fruit in ["apple", "banana", "orange"]:
    print(fruit)

# Using range()
for i in range(5):
    print(i)  # 0 1 2 3 4

# With enumerate (index + value)
for index, fruit in enumerate(["a", "b", "c"]):
    print(f"{index}: {fruit}")
```

**Break & Continue:**
```python
for i in range(10):
    if i == 3:
        break  # Exit loop
    if i == 1:
        continue  # Skip to next iteration
    print(i)  # 0 2
```

### Functions

```python
# BASIC FUNCTION
def greet(name):
    """This is a docstring"""
    return f"Hello, {name}!"

print(greet("Alice"))  # Hello, Alice!

# DEFAULT PARAMETERS
def add(a, b=0):
    return a + b

print(add(5))      # 5
print(add(5, 3))   # 8

# MULTIPLE RETURN VALUES
def divide_and_remainder(a, b):
    quotient = a // b
    remainder = a % b
    return quotient, remainder

q, r = divide_and_remainder(10, 3)
print(q, r)  # 3 1

# *ARGS (Variable number of arguments)
def sum_all(*args):
    total = 0
    for num in args:
        total += num
    return total

print(sum_all(1, 2, 3, 4))  # 10

# **KWARGS (Keyword arguments)
def print_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

print_info(name="Alice", age=25, city="NYC")
# name: Alice
# age: 25
# city: NYC

# LAMBDA (Anonymous function)
square = lambda x: x ** 2
print(square(5))  # 25

# HIGHER-ORDER FUNCTIONS
numbers = [1, 2, 3, 4, 5]
squared = list(map(lambda x: x**2, numbers))  # [1, 4, 9, 16, 25]
evens = list(filter(lambda x: x % 2 == 0, numbers))  # [2, 4]
```

### Exception Handling

```python
try:
    # Code that might cause an error
    result = 10 / 0
except ZeroDivisionError:
    # Specific error handling
    print("Cannot divide by zero!")
except Exception as e:
    # General error handling
    print(f"Error occurred: {e}")
else:
    # Runs if no exception
    print("Success!")
finally:
    # Always runs
    print("Cleanup code")
```

## 2.3 Common Programming Algorithms

### Sorting

```python
# BUBBLE SORT (Beginner, O(n²))
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n - i - 1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]
    return arr

print(bubble_sort([64, 34, 25, 12, 22, 11, 90]))
# [11, 12, 22, 25, 34, 64, 90]

# QUICK SORT (Advanced, O(n log n))
def quick_sort(arr):
    if len(arr) <= 1:
        return arr
    pivot = arr[len(arr) // 2]
    left = [x for x in arr if x < pivot]
    middle = [x for x in arr if x == pivot]
    right = [x for x in arr if x > pivot]
    return quick_sort(left) + middle + quick_sort(right)

# MERGE SORT (Advanced, O(n log n))
def merge_sort(arr):
    if len(arr) <= 1:
        return arr
    mid = len(arr) // 2
    left = merge_sort(arr[:mid])
    right = merge_sort(arr[mid:])
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
```

### Searching

```python
# LINEAR SEARCH (O(n))
def linear_search(arr, target):
    for i in range(len(arr)):
        if arr[i] == target:
            return i
    return -1

print(linear_search([10, 20, 30, 40, 50], 30))  # 2

# BINARY SEARCH (O(log n)) - Requires sorted array
def binary_search(arr, target):
    left, right = 0, len(arr) - 1
    while left <= right:
        mid = (left + right) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return -1

print(binary_search([10, 20, 30, 40, 50], 30))  # 2
```

### Recursion

```python
# FACTORIAL
def factorial(n):
    if n <= 1:
        return 1
    return n * factorial(n - 1)

print(factorial(5))  # 120

# FIBONACCI
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n - 1) + fibonacci(n - 2)

print(fibonacci(6))  # 8

# FIBONACCI (Optimized with Memoization)
def fibonacci_memo(n, memo={}):
    if n in memo:
        return memo[n]
    if n <= 1:
        return n
    memo[n] = fibonacci_memo(n - 1, memo) + fibonacci_memo(n - 2, memo)
    return memo[n]

print(fibonacci_memo(6))  # 8 (much faster)
```

---

# PART 3: DATA STRUCTURES & ALGORITHMS

## 3.1 Essential Data Structures

### Array/List
```python
arr = [1, 2, 3, 4, 5]

# Access: O(1)
print(arr[0])  # 1

# Insert: O(n)
arr.insert(2, 99)  # [1, 2, 99, 3, 4, 5]

# Delete: O(n)
arr.pop(2)  # [1, 2, 3, 4, 5]

# Search: O(n)
print(99 in arr)  # False
```

**Use When:** Need fast random access, don't know size in advance

### Linked List
```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None
    
    def insert_at_beginning(self, data):
        new_node = Node(data)
        new_node.next = self.head
        self.head = new_node
    
    def insert_at_end(self, data):
        new_node = Node(data)
        if not self.head:
            self.head = new_node
            return
        current = self.head
        while current.next:
            current = current.next
        current.next = new_node
    
    def display(self):
        elements = []
        current = self.head
        while current:
            elements.append(current.data)
            current = current.next
        print(" -> ".join(map(str, elements)))

ll = LinkedList()
ll.insert_at_end(1)
ll.insert_at_end(2)
ll.insert_at_end(3)
ll.display()  # 1 -> 2 -> 3
```

**Operations:**
- Insert at beginning: O(1)
- Insert at end: O(n)
- Delete: O(n)
- Search: O(n)

**Use When:** Frequent insertions/deletions, don't need random access

### Stack (LIFO - Last In First Out)
```python
class Stack:
    def __init__(self):
        self.items = []
    
    def push(self, item):
        self.items.append(item)
    
    def pop(self):
        return self.items.pop() if not self.is_empty() else None
    
    def peek(self):
        return self.items[-1] if not self.is_empty() else None
    
    def is_empty(self):
        return len(self.items) == 0

stack = Stack()
stack.push(1)
stack.push(2)
stack.push(3)
print(stack.pop())  # 3
print(stack.peek())  # 2
```

**Use Cases:** Undo/Redo, function call stack, expression evaluation, backtracking

### Queue (FIFO - First In First Out)
```python
from collections import deque

class Queue:
    def __init__(self):
        self.items = deque()
    
    def enqueue(self, item):
        self.items.append(item)
    
    def dequeue(self):
        return self.items.popleft() if not self.is_empty() else None
    
    def is_empty(self):
        return len(self.items) == 0

queue = Queue()
queue.enqueue(1)
queue.enqueue(2)
queue.enqueue(3)
print(queue.dequeue())  # 1
```

**Use Cases:** BFS, print job scheduling, customer service lines

### Hash Table / Dictionary
```python
# Python dictionaries are hash tables
hash_table = {}

# Insert: O(1) average
hash_table["name"] = "Alice"

# Lookup: O(1) average
print(hash_table["name"])  # Alice

# Delete: O(1) average
del hash_table["name"]

# Collision handling example (using linear probing)
class HashTable:
    def __init__(self, size=10):
        self.size = size
        self.table = [None] * size
    
    def hash(self, key):
        return hash(key) % self.size
    
    def insert(self, key, value):
        index = self.hash(key)
        while self.table[index] is not None:
            index = (index + 1) % self.size
        self.table[index] = (key, value)
    
    def lookup(self, key):
        index = self.hash(key)
        while self.table[index] is not None:
            if self.table[index][0] == key:
                return self.table[index][1]
            index = (index + 1) % self.size
        return None
```

**Use Cases:** Caching, counting frequencies, mapping relationships

### Tree
```python
class TreeNode:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

class BinarySearchTree:
    def __init__(self):
        self.root = None
    
    def insert(self, value):
        if not self.root:
            self.root = TreeNode(value)
        else:
            self._insert_recursive(self.root, value)
    
    def _insert_recursive(self, node, value):
        if value < node.value:
            if node.left is None:
                node.left = TreeNode(value)
            else:
                self._insert_recursive(node.left, value)
        else:
            if node.right is None:
                node.right = TreeNode(value)
            else:
                self._insert_recursive(node.right, value)
    
    def search(self, value):
        return self._search_recursive(self.root, value)
    
    def _search_recursive(self, node, value):
        if node is None:
            return False
        if node.value == value:
            return True
        elif value < node.value:
            return self._search_recursive(node.left, value)
        else:
            return self._search_recursive(node.right, value)

bst = BinarySearchTree()
for val in [50, 30, 70, 20, 40, 60, 80]:
    bst.insert(val)
print(bst.search(40))  # True
```

**Common Trees:**
- **Binary Search Tree:** Left < Parent < Right
- **AVL Tree:** Balanced BST
- **Red-Black Tree:** Self-balancing
- **B-Tree:** Multi-way tree (databases)

### Graph
```python
class Graph:
    def __init__(self):
        self.graph = {}
    
    def add_edge(self, u, v):
        if u not in self.graph:
            self.graph[u] = []
        self.graph[u].append(v)
    
    def dfs(self, node, visited=None):
        """Depth-First Search"""
        if visited is None:
            visited = set()
        visited.add(node)
        print(node, end=" ")
        for neighbor in self.graph.get(node, []):
            if neighbor not in visited:
                self.dfs(neighbor, visited)
    
    def bfs(self, start):
        """Breadth-First Search"""
        visited = set()
        queue = [start]
        visited.add(start)
        while queue:
            node = queue.pop(0)
            print(node, end=" ")
            for neighbor in self.graph.get(node, []):
                if neighbor not in visited:
                    visited.add(neighbor)
                    queue.append(neighbor)

g = Graph()
g.add_edge(0, 1)
g.add_edge(0, 2)
g.add_edge(1, 2)
g.add_edge(2, 3)

print("DFS:", end=" ")
g.dfs(0)  # 0 1 2 3
print("\nBFS:", end=" ")
g.bfs(0)  # 0 1 2 3
```

## 3.2 Big O Complexity Analysis

Understanding efficiency is crucial.

```
Complexity Order (Best to Worst):
O(1) < O(log n) < O(n) < O(n log n) < O(n²) < O(n³) < O(2ⁿ) < O(n!)
```

### Common Complexities

| Complexity | Time (1M items) | Example |
|-----------|-----------------|---------|
| O(1) | 1 nanosecond | Array access, hash lookup |
| O(log n) | 20 nanoseconds | Binary search |
| O(n) | 1 second | Linear search |
| O(n log n) | 20 seconds | Merge sort, quick sort |
| O(n²) | 12 days | Bubble sort, nested loops |
| O(2ⁿ) | Impossible | Brute force, subset generation |

### Analysis Examples

```python
# O(1) - Constant
def get_first_element(arr):
    return arr[0]

# O(n) - Linear
def sum_array(arr):
    total = 0
    for num in arr:
        total += num
    return total

# O(n²) - Quadratic
def bubble_sort(arr):
    for i in range(len(arr)):
        for j in range(len(arr) - 1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]

# O(log n) - Logarithmic
def binary_search(arr, target):
    left, right = 0, len(arr) - 1
    while left <= right:
        mid = (left + right) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return -1

# O(n log n) - Linearithmic
def merge_sort(arr):
    if len(arr) <= 1:
        return arr
    # ... (as shown before)
```

---

# PART 4: OBJECT-ORIENTED PROGRAMMING

## 4.1 OOP Fundamentals

### Classes and Objects

```python
class Dog:
    # Class variable (shared by all instances)
    species = "Canis familiaris"
    
    def __init__(self, name, age):
        # Instance variables
        self.name = name
        self.age = age
    
    def bark(self):
        return f"{self.name} says woof!"
    
    def __str__(self):
        return f"Dog(name='{self.name}', age={self.age})"
    
    def __repr__(self):
        return f"Dog('{self.name}', {self.age})"

# Creating objects (instances)
dog1 = Dog("Buddy", 3)
dog2 = Dog("Max", 5)

print(dog1.bark())  # Buddy says woof!
print(dog1.name)    # Buddy
print(Dog.species)  # Canis familiaris
```

### Inheritance

```python
class Animal:
    def __init__(self, name):
        self.name = name
    
    def make_sound(self):
        pass

class Dog(Animal):  # Inherits from Animal
    def make_sound(self):
        return f"{self.name} barks"

class Cat(Animal):  # Inherits from Animal
    def make_sound(self):
        return f"{self.name} meows"

dog = Dog("Buddy")
cat = Cat("Whiskers")

print(dog.make_sound())  # Buddy barks
print(cat.make_sound())  # Whiskers meows
```

### Polymorphism

```python
def animal_sound(animal):
    print(animal.make_sound())

dog = Dog("Buddy")
cat = Cat("Whiskers")

animal_sound(dog)   # Buddy barks
animal_sound(cat)   # Whiskers meows
```

### Encapsulation

```python
class BankAccount:
    def __init__(self, balance):
        self.__balance = balance  # Private attribute (double underscore)
    
    def deposit(self, amount):
        if amount > 0:
            self.__balance += amount
    
    def withdraw(self, amount):
        if 0 < amount <= self.__balance:
            self.__balance -= amount
    
    def get_balance(self):
        return self.__balance  # Controlled access

account = BankAccount(1000)
account.deposit(500)
print(account.get_balance())  # 1500
# print(account.__balance)    # AttributeError!
```

### Abstraction

```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass
    
    @abstractmethod
    def perimeter(self):
        pass

class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius
    
    def area(self):
        return 3.14 * self.radius ** 2
    
    def perimeter(self):
        return 2 * 3.14 * self.radius

circle = Circle(5)
print(circle.area())      # 78.5
print(circle.perimeter()) # 31.4
```

## 4.2 Advanced OOP Concepts

### Composition vs Inheritance

```python
# INHERITANCE (Is-A relationship)
class Vehicle:
    pass

class Car(Vehicle):  # Car IS A Vehicle
    pass

# COMPOSITION (Has-A relationship)
class Engine:
    def start(self):
        return "Engine started"

class Car:
    def __init__(self):
        self.engine = Engine()  # Car HAS AN Engine
    
    def start(self):
        return self.engine.start()
```

### Design Patterns (Brief Overview)

**Singleton Pattern:**
```python
class Database:
    _instance = None
    
    def __new__(cls):
        if cls._instance is None:
            cls._instance = super().__new__(cls)
        return cls._instance

db1 = Database()
db2 = Database()
print(db1 is db2)  # True (same instance)
```

**Observer Pattern:**
```python
class Subject:
    def __init__(self):
        self._observers = []
    
    def attach(self, observer):
        self._observers.append(observer)
    
    def notify(self, message):
        for observer in self._observers:
            observer.update(message)

class Observer:
    def update(self, message):
        print(f"Received: {message}")

subject = Subject()
observer1 = Observer()
observer2 = Observer()

subject.attach(observer1)
subject.attach(observer2)
subject.notify("Hello!")  # Both observers notified
```

---

# PART 5: DATABASES & SQL

## 5.1 Database Basics

### What is a Database?
Organized collection of structured data stored and accessed electronically.

### Types of Databases

#### 1. **Relational Databases (SQL)**
- Structured data in tables
- ACID compliance (Atomicity, Consistency, Isolation, Durability)
- Examples: MySQL, PostgreSQL, Oracle, SQL Server

```
┌─────────────────────┐
│      Students       │
├─────────────────────┤
│ ID | Name  | Grade  │
├─────────────────────┤
│ 1  | Alice | A      │
│ 2  | Bob   | B      │
│ 3  | Carol | A      │
└─────────────────────┘
```

#### 2. **NoSQL Databases**
- Flexible schema
- Horizontal scalability
- Types:
  - **Document (MongoDB):** JSON-like documents
  - **Key-Value (Redis):** Simple key-value pairs
  - **Graph (Neo4j):** Relationship-focused
  - **Column-Family (Cassandra):** Wide columns

### Normalization
Organizing data to reduce redundancy.

**1NF (First Normal Form):**
- Each cell contains single value
- No repeating groups

**2NF (Second Normal Form):**
- Meets 1NF
- No partial dependencies

**3NF (Third Normal Form):**
- Meets 2NF
- No transitive dependencies

## 5.2 SQL - Structured Query Language

### Creating Tables

```sql
CREATE TABLE students (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) UNIQUE,
    age INT CHECK (age >= 18),
    enrollment_date DATE DEFAULT CURRENT_DATE
);

CREATE TABLE courses (
    id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(100) NOT NULL,
    instructor VARCHAR(100),
    student_id INT,
    FOREIGN KEY (student_id) REFERENCES students(id)
);
```

### Basic CRUD Operations

```sql
-- CREATE (INSERT)
INSERT INTO students (name, email, age) 
VALUES ('Alice', 'alice@example.com', 20);

INSERT INTO students (name, email, age) 
VALUES 
    ('Bob', 'bob@example.com', 22),
    ('Carol', 'carol@example.com', 21);

-- READ (SELECT)
SELECT * FROM students;
SELECT name, email FROM students;
SELECT * FROM students WHERE age >= 21;
SELECT DISTINCT age FROM students;

-- UPDATE
UPDATE students 
SET age = 23 
WHERE name = 'Alice';

UPDATE students 
SET email = 'newemail@example.com' 
WHERE id = 1;

-- DELETE
DELETE FROM students WHERE id = 1;
```

### Filtering and Sorting

```sql
-- WHERE clause with conditions
SELECT * FROM students 
WHERE age > 20 AND name LIKE 'A%';

SELECT * FROM students 
WHERE age IN (20, 21, 22);

SELECT * FROM students 
WHERE age BETWEEN 20 AND 22;

-- ORDER BY
SELECT * FROM students 
ORDER BY age ASC;

SELECT * FROM students 
ORDER BY age DESC, name ASC;

-- LIMIT
SELECT * FROM students 
LIMIT 10;

SELECT * FROM students 
LIMIT 5 OFFSET 10;  -- Skip first 10, get next 5
```

### Aggregate Functions

```sql
SELECT COUNT(*) FROM students;              -- Total records
SELECT AVG(age) FROM students;               -- Average age
SELECT MAX(age), MIN(age) FROM students;     -- Max and min age
SELECT SUM(age) FROM students;               -- Sum of all ages

-- GROUP BY
SELECT age, COUNT(*) 
FROM students 
GROUP BY age;

SELECT age, COUNT(*) as student_count
FROM students 
GROUP BY age 
HAVING COUNT(*) > 1;
```

### Joins

```sql
-- INNER JOIN (only matching records)
SELECT students.name, courses.title
FROM students
INNER JOIN courses ON students.id = courses.student_id;

-- LEFT JOIN (all from left table)
SELECT students.name, courses.title
FROM students
LEFT JOIN courses ON students.id = courses.student_id;

-- RIGHT JOIN (all from right table)
SELECT students.name, courses.title
FROM students
RIGHT JOIN courses ON students.id = courses.student_id;

-- FULL OUTER JOIN (all from both)
SELECT students.name, courses.title
FROM students
FULL OUTER JOIN courses ON students.id = courses.student_id;

-- Self Join
SELECT a.name as employee, b.name as manager
FROM employees a
LEFT JOIN employees b ON a.manager_id = b.id;
```

### Subqueries

```sql
-- Subquery in WHERE
SELECT * FROM students
WHERE age > (SELECT AVG(age) FROM students);

-- Subquery in FROM
SELECT * FROM (
    SELECT name, age FROM students WHERE age > 20
) as young_students;

-- Correlated subquery
SELECT name FROM students s1
WHERE age > (SELECT AVG(age) FROM students s2 WHERE s2.age = s1.age);
```

### Indexes

```sql
-- Create index for faster queries
CREATE INDEX idx_email ON students(email);
CREATE INDEX idx_age_name ON students(age, name);

-- Drop index
DROP INDEX idx_email;
```

---

# PART 6: WEB DEVELOPMENT

## 6.1 Web Fundamentals

### HTTP (HyperText Transfer Protocol)

```
Client Request:
┌─────────────────────┐
│ HTTP Request        │
├─────────────────────┤
│ GET /users HTTP/1.1 │
│ Host: api.example   │
│ Content-Type: ...   │
└─────────────────────┘
           ↓
        Server
           ↓
┌─────────────────────┐
│ HTTP Response       │
├─────────────────────┤
│ HTTP/1.1 200 OK     │
│ Content-Type: JSON  │
│ {...data...}        │
└─────────────────────┘
```

### HTTP Methods

```
GET     - Retrieve data (safe, idempotent)
POST    - Create data
PUT     - Update entire resource
PATCH   - Update partial resource
DELETE  - Delete data
HEAD    - Like GET but no body
OPTIONS - Describe communication options
```

### Status Codes

```
1xx - Informational
2xx - Success (200 OK, 201 Created, 204 No Content)
3xx - Redirection (301 Moved, 302 Found)
4xx - Client Error (400 Bad Request, 401 Unauthorized, 403 Forbidden, 404 Not Found)
5xx - Server Error (500 Internal Server Error, 503 Service Unavailable)
```

## 6.2 Frontend Development

### HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Page Title</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="/">Home</a></li>
                <li><a href="/about">About</a></li>
            </ul>
        </nav>
    </header>
    
    <main>
        <section>
            <h1>Welcome</h1>
            <p>Content here</p>
        </section>
    </main>
    
    <footer>
        <p>&copy; 2026</p>
    </footer>
    
    <script src="script.js"></script>
</body>
</html>
```

### CSS Basics

```css
/* Selectors */
* { margin: 0; padding: 0; }                    /* All elements */
p { color: blue; }                               /* Element */
.container { width: 100%; }                     /* Class */
#header { background-color: gray; }             /* ID */
div > p { color: red; }                         /* Child */
div p { color: green; }                         /* Descendant */

/* Properties */
color: #FF5733;                  /* Text color */
background-color: #F0F0F0;      /* Background */
font-size: 16px;                /* Font size */
padding: 10px;                  /* Inside spacing */
margin: 20px;                   /* Outside spacing */
width: 100%;                    /* Width */
height: auto;                   /* Height */
display: flex;                  /* Layout */
justify-content: center;        /* Flex alignment */
border: 1px solid #ccc;         /* Border */
border-radius: 5px;             /* Rounded corners */
box-shadow: 0 2px 5px rgba();   /* Shadow */
transition: all 0.3s ease;      /* Animation */

/* Flexbox */
.flex-container {
    display: flex;
    justify-content: space-between;  /* Horizontal alignment */
    align-items: center;             /* Vertical alignment */
    gap: 10px;                       /* Space between items */
}

/* Grid */
.grid-container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;  /* 3 equal columns */
    gap: 20px;
}

/* Responsive */
@media (max-width: 768px) {
    .container {
        width: 90%;
    }
}
```

### JavaScript Basics

```javascript
// Variables
const PI = 3.14;           // Constant (preferred)
let name = "Alice";        // Block-scoped variable
var age = 25;              // Function-scoped (avoid)

// String manipulation
const greeting = `Hello, ${name}!`;
const text = "hello".toUpperCase();
const parts = "a,b,c".split(",");

// Arrays
const numbers = [1, 2, 3];
numbers.push(4);
numbers.pop();
numbers.map(n => n * 2);
numbers.filter(n => n > 2);

// Objects
const person = {
    name: "Alice",
    age: 25,
    greet() {
        return `Hi, I'm ${this.name}`;
    }
};

// DOM Manipulation
document.getElementById("myId").textContent = "Hello";
document.querySelector(".myClass").style.color = "red";
document.querySelectorAll("p").forEach(el => {
    el.addEventListener("click", () => {
        console.log("Clicked!");
    });
});

// Fetch API
fetch("https://api.example.com/users")
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error(error));

// Async/Await
async function getUsers() {
    try {
        const response = await fetch("https://api.example.com/users");
        const data = await response.json();
        return data;
    } catch (error) {
        console.error(error);
    }
}
```

## 6.3 Backend Development (Node.js/Express)

```javascript
const express = require('express');
const app = express();

// Middleware
app.use(express.json());
app.use(express.static('public'));

// Routes
app.get('/', (req, res) => {
    res.send('Welcome to the API');
});

app.get('/api/users', (req, res) => {
    const users = [
        { id: 1, name: 'Alice' },
        { id: 2, name: 'Bob' }
    ];
    res.json(users);
});

app.post('/api/users', (req, res) => {
    const newUser = req.body;
    // Save to database
    res.status(201).json(newUser);
});

app.get('/api/users/:id', (req, res) => {
    const userId = req.params.id;
    // Fetch from database
    res.json({ id: userId, name: 'Alice' });
});

app.put('/api/users/:id', (req, res) => {
    const userId = req.params.id;
    const updatedData = req.body;
    // Update in database
    res.json({ id: userId, ...updatedData });
});

app.delete('/api/users/:id', (req, res) => {
    const userId = req.params.id;
    // Delete from database
    res.status(204).send();
});

// Error handling
app.use((err, req, res, next) => {
    console.error(err.stack);
    res.status(500).json({ error: 'Internal Server Error' });
});

// Start server
app.listen(3000, () => {
    console.log('Server running on port 3000');
});
```

---

# PART 7: SYSTEM DESIGN & ARCHITECTURE

## 7.1 Scalability Concepts

### Vertical Scaling (Scale Up)
- Increase resources of single server
- Easier to implement
- Limited by hardware

```
Single Server (8GB RAM)
       ↓ (Add resources)
Single Server (32GB RAM)
```

### Horizontal Scaling (Scale Out)
- Add more servers
- Better for large-scale systems
- Requires load balancing

```
┌─────────────┐
│  Client     │
└──────┬──────┘
       │
    ┌──▼───┐
    │ Load │
    │Balancer
    └──┬────┘
       ├─────────────┬─────────────┐
       │             │             │
    ┌──▼──┐       ┌──▼──┐       ┌──▼──┐
    │ S1  │       │ S2  │       │ S3  │
    └─────┘       └─────┘       └─────┘
```

## 7.2 Caching Strategies

### Types of Caches

```
┌──────────────────────────────────────────┐
│ Client Cache (Browser)                   │ Fastest
├──────────────────────────────────────────┤
│ CDN Cache (Content Delivery Network)    │
├──────────────────────────────────────────┤
│ Application Cache (Redis, Memcached)    │
├──────────────────────────────────────────┤
│ Database Cache (Query Cache)            │
├──────────────────────────────────────────┤
│ Disk (SSD/HDD)                          │ Slowest
└──────────────────────────────────────────┘
```

### Cache Invalidation

```
1. Cache-Aside
   - Check cache first
   - If miss, fetch from DB and update cache
   - Application responsible for update

2. Write-Through
   - Write to cache and DB simultaneously
   - Ensures consistency
   - Slower writes

3. Write-Behind
   - Write to cache first, then DB asynchronously
   - Fast writes, but risk of data loss

4. Refresh-Ahead
   - Automatically refresh before expiration
   - Prevents cache misses
```

## 7.3 Database Scaling

### Sharding (Horizontal Partitioning)

```
Data distributed across multiple databases by key:

User IDs 1-1M → Database 1
User IDs 1M-2M → Database 2
User IDs 2M-3M → Database 3

Advantages:
- Distribute load
- Larger datasets
- Parallel queries

Disadvantages:
- Complex queries
- Hot spots
- Rebalancing difficult
```

### Replication

```
Master-Slave:
┌─────────┐         ┌─────────┐
│ Master  │────────→│ Slave 1 │
│ (Write) │         └─────────┘
└─────────┘         ┌─────────┐
     ↑──────────────│ Slave 2 │
     │              └─────────┘
  Reads from all
  
Master-Master:
┌─────────┐ ←────→ ┌─────────┐
│Master 1 │        │Master 2 │
└─────────┘        └─────────┘
(Both read/write, must handle conflicts)
```

---

# PART 8: OPERATING SYSTEMS

## 8.1 Processes and Threads

### Process
- Independent program instance
- Separate memory space
- Heavyweight (slow to create)

### Thread
- Lightweight process
- Shares memory with process
- Faster to create
- Risk of race conditions

```python
# THREADING EXAMPLE
import threading

def worker(name):
    print(f"Worker {name} starting")
    # Do work
    print(f"Worker {name} done")

threads = []
for i in range(5):
    t = threading.Thread(target=worker, args=(i,))
    threads.append(t)
    t.start()

for t in threads:
    t.join()  # Wait for all threads

print("All threads completed")
```

## 8.2 Memory Management

### Virtual Memory
```
Physical RAM:        Virtual Memory:
┌────────────┐      ┌──────────────────┐
│ Program A  │      │ Program A (RAM)  │
├────────────┤      ├──────────────────┤
│ Program B  │      │ Program B (RAM)  │
├────────────┤      ├──────────────────┤
│ Kernel     │      │ Program C (Disk) │
└────────────┘      └──────────────────┘

Larger than physical RAM
Managed by OS
Pages moved between RAM and disk (paging)
```

### Page Replacement Algorithms

```
LRU (Least Recently Used)
- Remove page not used for longest time
- Good locality of reference

FIFO (First In First Out)
- Simple to implement
- Poor performance

LFU (Least Frequently Used)
- Remove least frequently accessed
- Good cache performance
```

---

# PART 9: COMPUTER NETWORKS

## 9.1 OSI Model

```
7. Application    (HTTP, HTTPS, DNS, FTP, SMTP)
6. Presentation   (Encryption, Compression)
5. Session        (Connection management)
4. Transport      (TCP, UDP)
3. Network        (IP, Routing)
2. Data Link      (MAC, Ethernet)
1. Physical       (Cables, Signals)
```

## 9.2 TCP vs UDP

### TCP (Transmission Control Protocol)
```
Reliable, ordered, connection-oriented
- 3-way handshake (SYN, SYN-ACK, ACK)
- Guaranteed delivery
- Flow control
- Slower, more overhead

Use cases: Email, FTP, HTTP, Banking
```

### UDP (User Datagram Protocol)
```
Unreliable, connectionless, fast
- Sends datagrams without connection
- No guarantees
- Low overhead
- Faster, less reliable

Use cases: Video streaming, Gaming, VoIP, DNS
```

## 9.3 IP Addressing

```
IPv4: 192.168.1.1
     ││││││││││││││││────┬────┐
     └─ 32 bits total (4 octets)

Classes:
A: 1.0.0.0 - 126.255.255.255    (Large networks)
B: 128.0.0.0 - 191.255.255.255  (Medium networks)
C: 192.0.0.0 - 223.255.255.255  (Small networks)

Subnetting:
192.168.1.0/24
└─ /24 means first 24 bits are network, last 8 are host
   Supports 254 hosts (256 - 2 for network and broadcast)

IPv6: 2001:0db8:85a3:0000:0000:8a2e:0370:7334
     └─ 128 bits (supports many more addresses)
```

## 9.4 DNS (Domain Name System)

```
User enters URL:
example.com

     ↓ (DNS Query)
     
Recursive Resolver
     ↓ (asks)
Root Nameserver
     ↓ (refers to)
TLD Nameserver (.com)
     ↓ (refers to)
Authoritative Nameserver
     ↓ (returns IP)
93.184.216.34

Browser connects to IP
```

---

# PART 10: DEVOPS & CLOUD COMPUTING

## 10.1 Containerization (Docker)

```dockerfile
# Dockerfile
FROM python:3.9

WORKDIR /app

COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .

EXPOSE 5000

CMD ["python", "app.py"]
```

```bash
# Build image
docker build -t myapp:1.0 .

# Run container
docker run -p 5000:5000 myapp:1.0

# Docker Compose (multiple containers)
# docker-compose.yml
version: '3'
services:
  web:
    build: .
    ports:
      - "5000:5000"
  db:
    image: postgres:13
    environment:
      POSTGRES_DB: mydb
```

## 10.2 Cloud Platforms

### AWS (Amazon Web Services)
```
Compute:      EC2, Lambda, ECS
Storage:      S3, EBS, RDS
Networking:   VPC, CloudFront, Route 53
Databases:    RDS, DynamoDB, Aurora
```

### Azure (Microsoft)
```
Compute:      Virtual Machines, Azure Functions
Storage:      Blob Storage, Disk Storage
Database:     Azure SQL Database, Cosmos DB
```

### GCP (Google Cloud)
```
Compute:      Compute Engine, Cloud Functions
Storage:      Cloud Storage, Firestore
Database:     Cloud SQL, Bigtable
```

---

# PART 11: SECURITY & CRYPTOGRAPHY

## 11.1 Authentication & Authorization

### Authentication (Who are you?)
```
Password-based:
User → Password → Hash comparison → Access

Token-based (JWT):
User → Credentials → Token (encrypted) → Requests use token → Verify signature

Biometric:
Fingerprint/Face recognition → Access
```

### Authorization (What can you do?)
```
Role-Based Access Control (RBAC):
Admin   → Full access
User    → Limited access
Guest   → View only

Attribute-Based Access Control (ABAC):
Department: HR
Level: Senior
Location: HQ
→ Determine access based on attributes
```

## 11.2 Encryption

### Symmetric Encryption (Same key)
```
Plain text → Encrypt (key) → Cipher text → Decrypt (same key) → Plain text

Examples: AES, DES, RC4
Advantages: Fast, efficient
Disadvantages: Key distribution problem
```

### Asymmetric Encryption (Public/Private keys)
```
Public Key (shared):      Used to encrypt
Private Key (secret):     Used to decrypt

Plain text → Encrypt (public key) → Cipher text → Decrypt (private key) → Plain text

Examples: RSA, ECC
Advantages: Secure key exchange
Disadvantages: Slower than symmetric
```

### Hashing (One-way)
```
Input → Hash Function → Fixed output (Hash/Digest)
Cannot reverse
Used for: Passwords, checksums, signatures

Examples: MD5, SHA-1, SHA-256, bcrypt

Password storage:
1. User enters password
2. Hash with salt
3. Store hash (not password)
4. On login: Hash input, compare with stored
```

## 11.3 SSL/TLS (HTTPS)

```
HTTP (Insecure)
       ↓
HTTPS (HTTP + SSL/TLS)
       ↓
1. Client initiates secure connection
2. Server sends certificate
3. Client verifies certificate (issued by trusted CA)
4. Both establish shared encryption keys
5. Secure communication
```

---

# PART 12: SOFTWARE ENGINEERING BEST PRACTICES

## 12.1 Version Control (Git)

```bash
# Initialize repository
git init

# Basic workflow
git add filename          # Stage changes
git commit -m "Message"   # Commit changes
git push origin main      # Push to remote

# Branches
git branch feature         # Create branch
git checkout feature       # Switch branch
git merge feature          # Merge into main

# Collaboration
git pull                   # Get latest changes
git fetch                  # Download changes (no merge)
git rebase main            # Reapply commits on top of main
```

## 12.2 Code Quality

### Testing
```python
# Unit Testing
import unittest

class TestMath(unittest.TestCase):
    def test_add(self):
        self.assertEqual(2 + 2, 4)
    
    def test_subtract(self):
        self.assertEqual(5 - 2, 3)

if __name__ == '__main__':
    unittest.main()

# Integration Testing
# Test multiple components together

# End-to-End Testing
# Test entire application workflow
```

### Code Coverage
```
Percentage of code executed during testing
Target: 80%+ coverage
Tools: Coverage.py, Istanbul, JaCoCo
```

### SOLID Principles

```
S - Single Responsibility: One class, one responsibility
O - Open/Closed: Open for extension, closed for modification
L - Liskov Substitution: Derived classes substitute base classes
I - Interface Segregation: Specific interfaces, not general
D - Dependency Inversion: Depend on abstractions, not concretions
```

## 12.3 Debugging

```python
# Print debugging
print(f"Variable value: {x}")

# Using debugger
import pdb
pdb.set_trace()  # Breakpoint

# Logging
import logging
logging.basicConfig(level=logging.DEBUG)
logger = logging.getLogger(__name__)
logger.debug("Debug message")
logger.info("Info message")
logger.error("Error message")
```

---

# PART 13: ADVANCED TOPICS

## 13.1 Machine Learning Basics

```python
# Simple ML workflow
from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score

# Load data
iris = load_iris()
X = iris.data
y = iris.target

# Split data
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)

# Train model
model = RandomForestClassifier(n_estimators=100)
model.fit(X_train, y_train)

# Predict
predictions = model.predict(X_test)
accuracy = accuracy_score(y_test, predictions)
print(f"Accuracy: {accuracy}")
```

## 13.2 Concurrency & Async Programming

```python
# Asyncio
import asyncio

async def fetch_data(url):
    # Simulate API call
    await asyncio.sleep(1)
    return f"Data from {url}"

async def main():
    tasks = [
        fetch_data("url1"),
        fetch_data("url2"),
        fetch_data("url3")
    ]
    results = await asyncio.gather(*tasks)
    print(results)

asyncio.run(main())
```

## 13.3 Microservices Architecture

```
Monolithic:
┌─────────────────────────┐
│ Web Server              │
│ ├─ User Service        │
│ ├─ Product Service     │
│ ├─ Order Service       │
│ └─ Payment Service     │
└─────────────────────────┘

Microservices:
┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐
│ User     │  │ Product  │  │ Order    │  │ Payment  │
│ Service  │  │ Service  │  │ Service  │  │ Service  │
└──────────┘  └──────────┘  └──────────┘  └──────────┘
    ↑              ↑              ↑              ↑
    └──────────────┴──────────────┴──────────────┘
                    API Gateway
```

---

# LEARNING RESOURCES & TOOLS

## Online Platforms
- **Codecademy**: Interactive coding lessons
- **LeetCode**: Algorithm practice
- **HackerRank**: Programming challenges
- **Coursera**: University-level courses
- **Udemy**: Affordable, comprehensive courses
- **MIT OpenCourseWare**: Free university lectures
- **freeCodeCamp**: YouTube comprehensive tutorials

## Essential Tools
- **IDE**: VS Code, PyCharm, IntelliJ
- **Terminal**: Bash, PowerShell, Zsh
- **Version Control**: Git, GitHub, GitLab
- **Database**: MySQL, PostgreSQL, MongoDB
- **Package Manager**: npm, pip, Maven
- **Build Tools**: Docker, Jenkins, GitHub Actions

## Books
- "Clean Code" - Robert Martin
- "Design Patterns" - Gang of Four
- "Introduction to Algorithms" - CLRS
- "System Design Interview" - Alex Xu
- "The Pragmatic Programmer" - Hunt & Thomas

---

# INTERVIEW PREPARATION GUIDE

## 80/20 Focus Areas

### **Must Know (40% of interviews)**
1. Array/String manipulation
2. Binary search
3. Hash tables
4. Linked lists
5. Sorting and searching
6. Basic graphs (DFS, BFS)

### **Important (30% of interviews)**
1. Trees and BSTs
2. Dynamic programming
3. Recursion
4. Stack/Queue
5. Bit manipulation

### **Nice to Know (20% of interviews)**
1. Advanced graphs
2. Segment trees
3. Tries
4. Heap

### **System Design (10% of interviews)**
1. Scalability
2. Load balancing
3. Caching strategies
4. Database design

## Common Interview Patterns

### Two-Pointer Technique
```python
def two_sum_sorted(arr, target):
    left, right = 0, len(arr) - 1
    while left < right:
        current_sum = arr[left] + arr[right]
        if current_sum == target:
            return [left, right]
        elif current_sum < target:
            left += 1
        else:
            right -= 1
    return []
```

### Sliding Window
```python
def max_subarray_sum(arr, k):
    max_sum = sum(arr[:k])
    current_sum = max_sum
    
    for i in range(k, len(arr)):
        current_sum = current_sum - arr[i - k] + arr[i]
        max_sum = max(max_sum, current_sum)
    
    return max_sum
```

### Dynamic Programming
```python
def fibonacci(n, memo={}):
    if n in memo:
        return memo[n]
    if n <= 1:
        return n
    memo[n] = fibonacci(n - 1, memo) + fibonacci(n - 2, memo)
    return memo[n]
```

## Interview Tips

1. **Clarify the problem** - Ask questions before coding
2. **Explain your approach** - Walk through your solution
3. **Start simple** - Get brute force working first
4. **Optimize gradually** - Improve after basic solution works
5. **Test with examples** - Use different test cases
6. **Time complexity** - Always discuss O(n) analysis
7. **Edge cases** - Handle null, empty, single elements
8. **Code clarity** - Use meaningful variable names
9. **Communicate** - Think out loud
10. **Practice** - Solve 100+ problems before interviews

## 30-Day Preparation Plan

**Week 1: Fundamentals**
- Arrays and strings
- Basic sorting and searching
- Complexity analysis

**Week 2: Data Structures**
- Linked lists
- Stacks and queues
- Hash tables

**Week 3: Trees and Graphs**
- Binary trees
- Binary search trees
- Graph traversal (DFS, BFS)

**Week 4: Advanced**
- Dynamic programming
- Bit manipulation
- System design basics

---

## 🎯 Quick Reference Cheat Sheet

### Time Complexities
| Operation | Array | Linked List | Hash Table | BST |
|-----------|-------|-------------|------------|-----|
| Access | O(1) | O(n) | N/A | O(log n) |
| Search | O(n) | O(n) | O(1)* | O(log n) |
| Insert | O(n) | O(1) | O(1)* | O(log n) |
| Delete | O(n) | O(1) | O(1)* | O(log n) |

*Average case

### Key Formulas
```
Arithmetic Series: 1+2+...+n = n(n+1)/2
Geometric Series: 1+2+4+...+2^n = 2^(n+1) - 1
Permutations: P(n,r) = n! / (n-r)!
Combinations: C(n,r) = n! / (r!(n-r)!)
```

---

## 📈 Progression Path

**Month 1-2: Foundations**
- Programming basics
- Data structures
- Algorithm complexity

**Month 3-4: Problem Solving**
- Medium difficulty problems
- Interview patterns
- Optimization techniques

**Month 5-6: System Design**
- Scalability
- Database design
- Network architecture

**Month 7-12: Specialization**
- Web development OR
- DevOps OR
- Machine Learning OR
- Mobile development

---
