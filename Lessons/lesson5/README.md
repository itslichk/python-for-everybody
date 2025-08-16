# 🐍 Python for Everybody – Lesson 5: Repeating Actions with Loops (`while` and `for`)

Welcome to Lesson 5! 🎉  
You’ve learned how to make decisions with `if`, `else`, and `elif`. Now it’s time to teach your program how to **repeat actions** using loops. Loops are the backbone of automation and dynamic programming.

In this lesson, you’ll learn how to use `while` and `for` loops to run code multiple times—until a condition is met or through a sequence of items.

---

## 🎯 Learning Objectives

By the end of this lesson, you will be able to:

- Use `while` loops to repeat code based on a condition  
- Use `for` loops to iterate over sequences  
- Understand loop control with `break` and `continue`  
- Write programs that repeat tasks automatically

---

## 🔁 What is a Loop?

A **loop** lets your program repeat a block of code multiple times.  
There are two main types:

- `while` loop: repeats while a condition is `True`  
- `for` loop: repeats over a sequence (like a list or range)

---

## 🔄 `while` Loop

Repeats as long as the condition is `True`.

### ✅ Syntax

```python
while condition:
    # code to repeat
```

### 🧪 Example:

```python
count = 1
while count <= 5:
    print("Count:", count)
    count += 1
```

This prints numbers from 1 to 5.

---

## 🧠 Be Careful: Infinite Loops

If the condition never becomes `False`, the loop runs forever.

### ❌ Example:

```python
while True:
    print("This never stops!")  # Press Ctrl+C to stop
```

Always make sure your loop has an **exit condition**.

---

## 🔁 `for` Loop

Repeats over a sequence like a list or a range of numbers.

### ✅ Syntax

```python
for item in sequence:
    # code to repeat
```

### 🧪 Example:

```python
for i in range(5):
    print("i =", i)
```

This prints numbers from 0 to 4.

---

## 🔢 Using `range()`

The `range()` function generates a sequence of numbers.

```python
range(5)        # 0 to 4
range(1, 6)     # 1 to 5
range(0, 10, 2) # 0, 2, 4, 6, 8
```

---

## 🧪 Loop Control: `break` and `continue`

### 🔹 `break`: Exit the loop early

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

### 🔹 `continue`: Skip the current iteration

```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

---

## 🧪 Practice Exercises

### 📝 Exercise 1: Countdown

Write a program that:

- Asks for a number  
- Counts down to 0 using a `while` loop  
- Prints `"Blast off!"` at the end

---

### 📝 Exercise 2: Multiplication Table

Write a program that:

- Asks for a number  
- Prints its multiplication table from 1 to 10 using a `for` loop

---

## 🧪 Mini Project: Password Retry System

Create a program that:

1. Asks for a password  
2. Allows up to 3 attempts  
3. Prints `"Access granted"` if correct, or `"Access denied"` after 3 tries

### ✅ Example:

```python
correct_password = "python123"
attempts = 0

while attempts < 3:
    guess = input("Enter password: ")
    if guess == correct_password:
        print("Access granted.")
        break
    else:
        print("Wrong password.")
        attempts += 1

if attempts == 3:
    print("Access denied.")
```

---

## 💬 Instructor Note

> "Loops are what make your programs dynamic and powerful. Whether you're building a game, processing data, or automating tasks, loops are your best friend. Practice them well—they’re everywhere in real-world code."

---

## ⏭️ What’s Next?

In **Lesson 6**, we’ll explore:

- Functions: how to organize your code  
- Writing reusable blocks of logic  
- Making your programs cleaner and smarter

---

## 📚 Bonus Resources

- [Python Docs – `while` and `for` Loops](https://docs.python.org/3/tutorial/controlflow.html#for-statements)
- [Python Tutor – Visualize Loops](https://pythontutor.com/)

---

## 🙌 Keep Going!

You’ve now learned how to repeat actions and control the flow of your program.  
Loops are essential for building real applications—keep experimenting and looping your way to mastery!