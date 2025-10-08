# 🧱 Functions Learning Path — Year 9 Programmer

A complete step-by-step worksheet to master **Python functions** before moving into **Object-Oriented Programming (OOP).**

---

## 🧱 STAGE 1: Understanding Functions  
🎯 **Goal:**  
Learn how to define, call, and use parameters and return values in Python functions.

---

### 🧩 Task 1 — Your First Function
Define a function called `say_hello()` that prints:  
`"Hello, welcome to programming!"`  
Then call it.

```python
def say_hello():
    print("Hello, welcome to programming!")

say_hello()
```

---

### 🧩 Task 2 — Functions with Parameters
Create a function called `greet_user(name)` that prints a greeting using their name.  
**Example:**
```python
greet_user("Alex")  
# Output: Hello, Alex!
```

---

### 🧩 Task 3 — Functions with Return Values
Write a function called `add_numbers(a, b)` that returns their sum.  
**Example:**
```python
result = add_numbers(5, 3)
print(result)  # 8
```

---

### 🧩 Task 4 — Using Variables with Functions
Write a function called `area_of_rectangle(length, width)` that returns the area.  
Ask the user for input and print the result.

---

### 🧩 Task 5 — Default Parameters
Make a function `greet_user(name="friend")`.  
If no name is given, it should greet “friend”.

---

## 🧠 STAGE 2: Functions That Do Things  
🎯 **Goal:**  
Use functions to structure small programs and separate logic into smaller chunks.

---

### 🧩 Task 6 — A Simple Calculator
Create 4 functions:
- `add(a, b)`
- `subtract(a, b)`
- `multiply(a, b)`
- `divide(a, b)`

Then write a **main function** that asks the user what they want to do and calls the correct one.

---

### 🧩 Task 7 — Average of a List
Write a function `average(numbers)` that returns the average of a list of numbers.  
Then test it with `[10, 20, 30, 40]`.

---

### 🧩 Task 8 — Even or Odd Checker
Make a function `is_even(number)` that returns `True` if even, `False` if odd`.  
Then loop through numbers 1–10 and print the result for each.

---

### 🧩 Task 9 — Word Counter
Write a function `count_words(sentence)` that counts how many words are in a string.  
💡 *Hint:* use `.split()`.

---

### 🧩 Task 10 — Palindrome Checker
Create a function `is_palindrome(word)` that returns `True` if a word reads the same backwards.  
**Example:**  
`is_palindrome("racecar") → True`

---

## ⚙️ STAGE 3: Problem Solving with Functions  
🎯 **Goal:**  
Apply logic, loops, and conditionals inside functions — closer to how you’ll design methods later in OOP.

---

### 🧩 Task 11 — Temperature Converter
Write two functions:
- `c_to_f(celsius)`
- `f_to_c(fahrenheit)`  
Then make a small program that asks what the user wants to convert.

---

### 🧩 Task 12 — Prime Number Checker
Write a function `is_prime(number)` that returns `True` if the number is prime.

---

### 🧩 Task 13 — Factorial Function
Write a function `factorial(n)` that returns `n!` using a loop.

---

### 🧩 Task 14 — Random Password Generator
Write a function `generate_password(length)` that creates a random string using letters and numbers.  
💡 *Hint:* use the `random` and `string` modules.

---

### 🧩 Task 15 — Menu System
Create a function `main_menu()` that prints a menu (e.g., “1. Add Task, 2. View Tasks, 3. Quit”).  
Keep it looping until the user chooses to quit.  
👉 This introduces control flow, useful for later OOP programs.

---

## 🚀 STAGE 4: Functions Working Together (Mini-Projects)  
🎯 **Goal:**  
Get used to organizing multiple functions into a single working system.

---

### 🧩 Project 1 — To-Do List Manager
Functions:
- `add_task(task_list, task)`
- `view_tasks(task_list)`
- `remove_task(task_list, index)`  
Use a list to store tasks and call functions from a menu loop.

---

### 🧩 Project 2 — Quiz Game
Functions:
- `ask_question(question, answer)`
- `run_quiz()`  
Store questions in a list of tuples and loop through them.

---

### 🧩 Project 3 — Guess the Number
Functions:
- `generate_number()`
- `get_guess()`
- `check_guess(secret, guess)`

---

### 🧩 Project 4 — Rock, Paper, Scissors
Functions:
- `get_user_choice()`
- `get_computer_choice()`
- `decide_winner(user, computer)`

---

## 🔗 Transition to OOP
Once you’ve completed these tasks, you’ll naturally start thinking:  
> “Hmm, what if I grouped all my related functions and data together?”  

That’s the perfect moment to introduce **classes** — starting with something like turning the “Dog” or “Calculator” into a class.
