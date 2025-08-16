# 🧠 Lesson 10: Error Handling in Python – Writing Smarter Code

🎉 Congratulations! You’ve made it to the final lesson of the course.  
You’ve learned how to write programs, use variables, control flow, work with data structures, and even read and write files.

Now it’s time to learn how to make your programs **robust**—so they don’t crash when something goes wrong.  
This lesson introduces **error handling**, a key skill for writing professional, user-friendly code.

---

## 🎯 Objectives

By the end of this final lesson, you’ll be able to:

- Understand what errors are and why they happen  
- Use `try`, `except`, and `finally` to handle errors gracefully  
- Prevent your programs from crashing unexpectedly  
- Write code that’s more reliable and easier to debug

---

## ⚠️ What Is an Error?

Errors are problems that occur while your program is running.  
Some common types:

- `ZeroDivisionError` – Dividing by zero  
- `ValueError` – Invalid value (e.g. converting "abc" to int)  
- `FileNotFoundError` – Trying to open a file that doesn’t exist

---

## 🛡️ Using `try` and `except`

Python lets you catch errors using `try` and `except`.

```python
try:
    number = int(input("Enter a number: "))
    result = 10 / number
    print("Result:", result)
except ZeroDivisionError:
    print("You can't divide by zero!")
except ValueError:
    print("Please enter a valid number.")
```

---

## 🔄 Optional: `finally` Block

Use `finally` to run code no matter what happens.

```python
try:
    file = open("data.txt", "r")
    content = file.read()
except FileNotFoundError:
    print("File not found.")
finally:
    print("Program finished.")
```

---

## 🧪 Practice Exercises

### 📝 Exercise 1: Safe Calculator

Write a program that:

- Asks the user for two numbers  
- Divides them  
- Handles division by zero and invalid input

---

### 📝 Exercise 2: File Reader with Grace

Ask the user for a filename.  
Try to open and read it.  
If the file doesn’t exist, show a friendly message.

---

## 🛠️ Final Project: Smart Contact Saver

Build a program that:

1. Asks the user for a name and phone number  
2. Saves it to `contacts.txt`  
3. Handles errors like missing input or file issues

```python
try:
    name = input("Enter name: ")
    phone = input("Enter phone: ")

    if not name or not phone:
        raise ValueError("Name and phone cannot be empty.")

    with open("contacts.txt", "a") as file:
        file.write(f"{name}: {phone}\n")
    print("Contact saved!")
except ValueError as e:
    print("Error:", e)
except Exception as e:
    print("Something went wrong:", e)
```

---

## 💬 Final Instructor Message

> “You’ve come so far. From printing your first message to building real programs that handle errors and save data.  
> You now have the tools to keep learning, building, and solving problems with Python.  
> Keep coding, keep experimenting, and most importantly—keep helping others through what you create.”

---

## 🎓 What’s Next?

You’ve completed the **Python for Everybody** course!  
Here are some ideas for your next steps:

- Build a portfolio of mini-projects  
- Explore web development with Flask or Django  
- Learn about APIs and automation  
- Teach others what you’ve learned!

---

## 🏁 Final Words

This is just the beginning.  
You now have the power to build tools, solve problems, and create value with code.  
Thank you for learning with us—and remember: **every great developer started where you are now.**

Keep going. The world needs your ideas. 🌍💡