# 🐍 Python for Everybody – Lesson 6: Organizing Code with Functions

Welcome to Lesson 6! 🎉  
You’ve learned how to write code that makes decisions and repeats actions. Now it’s time to learn how to **organize your code** using functions. Functions are reusable blocks of logic that make your programs cleaner, smarter, and easier to manage.

---

## 🎯 Learning Objectives

By the end of this lesson, you will be able to:

- Define and call functions in Python  
- Use parameters and return values  
- Understand the difference between local and global variables  
- Write reusable, modular code

---

## 🧩 What is a Function?

A **function** is a named block of code that performs a specific task.  
You can call it whenever you need it—no need to rewrite the same logic again and again.

---

## ✅ Defining a Function

Use the `def` keyword to define a function.

```python
def greet():
    print("Hello, world!")
```

### 🔹 Calling the Function

```python
greet()
```

This prints:  
```
Hello, world!
```

---

## 🎯 Parameters: Passing Information

You can pass data into a function using **parameters**.

### ✅ Example:

```python
def greet(name):
    print("Hello, " + name + "!")
```

```python
greet("Ryan")
```

This prints:  
```
Hello, Ryan!
```

---

## 🔙 Return Values: Getting Results

Use `return` to send a result back from a function.

### ✅ Example:

```python
def add(a, b):
    return a + b

result = add(3, 5)
print("Sum:", result)
```

This prints:  
```
Sum: 8
```

---

## 🧠 Local vs Global Variables

Variables inside a function are **local**—they exist only inside that function.

### ✅ Example:

```python
def show_message():
    message = "Hello from inside!"
    print(message)

show_message()
# print(message)  ❌ Error: message is not defined outside
```

---

## 🧪 Practice Exercises

### 📝 Exercise 1: Calculator Function

Write a function `calculate()` that:

- Takes two numbers and an operator (`+`, `-`, `*`, `/`)  
- Returns the result

---

### 📝 Exercise 2: Temperature Converter

Write a function `celsius_to_fahrenheit(c)` that:

- Converts Celsius to Fahrenheit using the formula: `F = C * 9/5 + 32`  
- Returns the result

---

## 🧪 Mini Project: Personalized Greeting System

Create a program that:

1. Defines a function `greet_user(name, age)`  
2. Prints a personalized message like: `"Hello Ryan, you are 21 years old!"`  
3. Calls the function with user input

### ✅ Example:

```python
def greet_user(name, age):
    print("Hello " + name + ", you are " + str(age) + " years old!")

user_name = input("Enter your name: ")
user_age = int(input("Enter your age: "))
greet_user(user_name, user_age)
```

---

## 💬 Instructor Note

> "Functions are the building blocks of clean code. They help you break down problems, reuse logic, and write programs that scale. Once you master functions, you’re thinking like a real developer."

---

## ⏭️ What’s Next?

In **Lesson 7**, we’ll explore:

- Lists: how to store multiple values  
- Looping through lists  
- Building programs that handle collections of data

---

## 📚 Bonus Resources

- [Python Docs – Functions](https://docs.python.org/3/tutorial/controlflow.html#defining-functions)
- [Python Tutor – Visualize Functions](https://pythontutor.com/)

---

## 🙌 Keep Going!

You’ve now learned how to write reusable, organized code using functions.  
This is a huge step toward building real-world applications. Keep practicing and modularizing your logic—you’re becoming a true Pythonista!