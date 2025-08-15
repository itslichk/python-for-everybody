# 🐍 Python for Everybody – Lesson 2: Variables and Data Types

Welcome back! 🎉  
In Lesson 1, you learned how to use `print()` and `input()` to communicate with your computer. Now it’s time to learn how Python **stores and manages information** using variables and data types.

This lesson is all about giving your data a name and understanding how Python thinks about different kinds of information.

---

## 🎯 Learning Objectives

By the end of this lesson, you will be able to:

- Create and use variables  
- Understand and use basic data types: `str`, `int`, `float`, and `bool`  
- Convert between data types  
- Write programs that store and manipulate user input

---

## 📦 What is a Variable?

A **variable** is like a labeled box where you store information. You give it a name, and Python remembers what’s inside.

### ✅ Syntax

```python
name = "Ryan"
age = 21
```

Here, `name` stores a string, and `age` stores a number.

---

## 🔤 Data Types in Python

Python has several built-in data types. Here are the most common ones for beginners:

| Type   | Example       | Description                     |
|--------|---------------|---------------------------------|
| `str`  | `"Hello"`     | Text (string of characters)     |
| `int`  | `42`          | Whole number (integer)          |
| `float`| `3.14`        | Decimal number (floating point) |
| `bool` | `True`, `False` | Logical value (true/false)    |

---

## 🧪 Examples

```python
name = "Ryan"        # str
age = 21             # int
height = 1.75        # float
is_student = True    # bool
```

You can use these variables in your program:

```python
print("Name:", name)
print("Age:", age)
print("Height:", height)
print("Student:", is_student)
```

---

## 🔄 Getting Input and Converting Types

Remember: `input()` always returns a string.  
To use numbers, you need to convert them.

### ✅ Example:

```python
age = input("How old are you? ")
print("Next year, you'll be", int(age) + 1)
```

Here, `int(age)` converts the string to an integer so we can do math.

---

## 🔁 Type Conversion Functions

| Function   | Converts to... |
|------------|----------------|
| `int()`    | Integer         |
| `float()`  | Decimal         |
| `str()`    | String          |
| `bool()`   | Boolean         |

### 🧪 Example:

```python
price = float(input("Enter the price: "))
print("Price with tax:", price * 1.19)
```

---

## 🧠 Concept Check

Try answering these:

1. What is a variable?
2. What data type does `input()` return?
3. How do you convert `"42"` to a number?
4. What’s the difference between `int` and `float`?

---

## 🧪 Practice Exercises

### 📝 Exercise 1: Age Calculator

Write a program that:

- Asks for the user's birth year  
- Calculates their age  
- Prints: `"You are [age] years old."`

Hint: Use `int()` and subtract from the current year.

---

### 📝 Exercise 2: BMI Calculator

Write a program that:

- Asks for height (in meters) and weight (in kg)  
- Calculates BMI: `weight / (height ** 2)`  
- Prints the result

---

## 🧪 Mini Project: Personal Profile Generator

Create a program that:

1. Asks for name, age, height, and student status  
2. Converts age and height to numbers  
3. Prints a formatted profile

### ✅ Example Output:

```
What's your name? Ryan  
How old are you? 21  
How tall are you (in meters)? 1.75  
Are you a student? True  

--- Profile ---
Name: Ryan  
Age: 21  
Height: 1.75 m  
Student: True
```

---

## 💬 Instructor Note

> "Variables are the memory of your program. They let you store, reuse, and manipulate data. Once you understand how Python handles different types of information, you can start building logic and intelligence into your code."

---

## ⏭️ What’s Next?

In **Lesson 3**, we’ll explore:

- Operators and expressions  
- How to do math and logic in Python  
- Writing smarter, more dynamic programs

---

## 📚 Bonus Resources

- [Python Docs – Built-in Types](https://docs.python.org/3/library/stdtypes.html)
- [Python Docs – Type Conversion](https://docs.python.org/3/library/functions.html)

---

## 🙌 Keep Going!

You’ve now learned how to store and manage data in Python. That’s a huge step toward building real applications.  
Practice, experiment, and don’t be afraid to break things. That’s how great coders learn!
