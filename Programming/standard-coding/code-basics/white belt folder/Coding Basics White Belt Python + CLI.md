<details>
<summary><h1>Coding Basics/White Belt/Python + CLI</h1></summary>

💡 Tip: Click the arrows next to each heading to expand or collapse the content underneath.

<details>
<summary><h2>Key Concepts</h2></summary>

<details>
<summary><h3>🔹 Variables and Constants (10)</h3></summary>

**Q1: What is a variable?**

A: A box that stores information, like a name tag holding a value.

**Q2: Why use variables?**

A: So you don’t have to retype numbers or words many times—you just save them once.

**Q3: How do you make a variable in Python?**

A: `age = 10`

**Q4: Can a variable change later?**

A: Yes, you can give it a new value. Example:

```python
age = 10
age = 11
```

**Q5: What is a constant?**

A: A value that should stay the same, like `PI = 3.14`.

**Q6: Does Python have real constants?**

A: No, but programmers write constants in ALL CAPS to remind themselves.

**Q7: When do you use a variable?**

A: When you need to remember something and might change it later.

**Q8: When do you use a constant?**

A: When you never want the value to change.

**Q9: Can variables hold text?**

A: Yes, like `name = "Alex"`.

**Q10: Can variables hold numbers?**

A: Yes, like `score = 50`.

</details>

---

<details>
<summary><h3>🔹 Data Types (Numbers, Strings, Booleans) (10)</h3></summary>

**Q11: What is a data type?**

A: It tells Python what kind of value something is.

**Q12: What is a number type?**

A: Values you can count or calculate, like `5` or `3.14`.

**Q13: What is a string?**

A: Text inside quotes, like `"Hello"`.

**Q14: What is a boolean?**

A: A truth value: `True` or `False`.

**Q15: Why do we need data types?**

A: So Python knows what kind of work to do with the value.

**Q16: How do you check a type?**

A: `print(type(5))` → `<class 'int'>`

**Q17: Can you add strings together?**

A: Yes, `"Hi" + " there"` → `"Hi there"`.

**Q18: Can you add numbers to strings directly?**

A: No, `"Hi" + 5` gives an error.

**Q19: How do you turn numbers into strings?**

A: `str(5)` → `"5"`.

**Q20: How do you turn strings into numbers?**

A: `int("5")` → `5`.

</details>

---

<details>
<summary><h3>🔹 Input/Output (10)</h3></summary>

**Q21: What is output?**

A: Showing information to the screen.

**Q22: How do you output in Python?**

A: `print("Hello")`

**Q23: What is input?**

A: Asking the user to type something.

**Q24: How do you take input in Python?**

A: `name = input("Enter your name: ")`

**Q25: What does input always give you?**

A: A string, even if you typed a number.

**Q26: How do you turn input into a number?**

A: `age = int(input("Enter your age: "))`

**Q27: Why use print()?**

A: To check what’s happening or to talk to the user.

**Q28: Why use input()?**

A: To let the user control the program.

**Q29: Can you print variables?**

A: Yes, `print(name)`

**Q30: Can you mix text and variables in print?**

A: Yes, `print("Hello", name)`

</details>

---

<details>
<summary><h3>🔹 Basic Math Operations (10)</h3></summary>

**Q31: How do you add in Python?**

A: `3 + 2` → `5`

**Q32: How do you subtract?**

A: `5 - 2` → `3`

**Q33: How do you multiply?**

A: `4 * 3` → `12`

**Q34: How do you divide?**

A: `10 / 2` → `5.0`

**Q35: What’s the difference between `/` and `//`?**

A: `/` gives decimals, `//` gives whole-number floor division results.

**Q36: How do you get the remainder?**

A: `%` → `7 % 3` → `1`

**Q37: How do you do powers?**

A: `2 ** 3` → `8`

**Q38: Can you use math with variables?**

A: Yes, `x = 5; y = 2; print(x + y)`

**Q39: Why use math operations?**

A: To calculate results instead of doing it by hand.

**Q40: Can you use math on strings?**

A: You can multiply a string: `"hi" * 3` → `"hihihi"`.

</details>

---

<details>
<summary><h3>🔹 Conditionals (if/else) (10)</h3></summary>

**Q51: What is a conditional?**

A: A rule that decides if code should run.

**Q52: How do you write an if statement?**

A:

```python
if age > 18:
    print("Adult")
```

**Q53: What does else mean?**

A: “Do this if the first rule is not true.”

**Q54: How do you write if/else?**

A:

```python
if age > 18:
    print("Adult")
else:
    print("Child")
```

**Q55: What does `elif` mean?**

A: “Try another rule.”

**Q56: Why use conditionals?**

A: To make decisions in your code.

**Q57: Can conditionals use booleans?**

A: Yes, `if True:` always runs.

**Q58: Can conditionals check strings?**

A: Yes, `if name == "Alex":`

**Q59: Can conditionals check multiple things?**

A: Yes, with `and` / `or`. Example:

```python
if age > 18 and age < 30:
    print("Young adult")
```

**Q60: What happens if no condition matches?**

A: Python skips the conditional branch unless you wrote an `else`.

</details>

</details>

<details>
<summary><h2>Code Syntax</h2></summary>

<details>
<summary><h3>Variables & Constants</h3></summary>

**Q1: How do I create a variable that stores a player's score?**

```python
score = 0
```

**Q2: How do I create a constant for an app name?**

```python
APP_NAME = "My CLI App"
```

**Q3: How do I store a user's name?**

```python
name = "John"
```

**Q4: How do I update a score variable?**

```python
score = score + 1
```

**Q5: How do I reset a variable to zero?**

```python
score = 0
```

**Q6: How do I copy one variable into another?**

```python
backup = score
```

**Q7: How do I store a game status as a variable?**

```python
is_running = True
```

**Q8: How do I change a variable based on a condition later?**

```python
score = score + 10
```

**Q9: How do I store a message in a variable?**

```python
message = "Hello Player"
```

**Q10: How do I define a constant for max score?**

```python
MAX_SCORE = 100
```

</details>

<details>
<summary><h3>Data Types</h3></summary>

**Q11: How do I store an integer number?**

```python
age = 25
```

**Q12: How do I store a decimal number?**

```python
price = 9.99
```

**Q13: How do I store text?**

```python
name = "Alice"
```

**Q14: How do I store a true/false value?**

```python
is_alive = True
```

**Q15: How do I convert input into an integer?**

```python
number = int(input())
```

**Q16: How do I convert input into a float?**

```python
number = float(input())
```

**Q17: How do I store multiple words in a string?**

```python
message = "Hello World"
```

**Q18: How do I check a variable type?**

```python
type(score)
```

**Q19: How do I store a negative number?**

```python
value = -5
```

**Q20: How do I convert a number to a string?**

```python
str(score)
```

</details>

<details>
<summary><h3>Input / Output</h3></summary>

**Q21: How do I print a message?**

```python
print("Hello World")
```

**Q22: How do I print a variable?**

```python
print(score)
```

**Q23: How do I get user input?**

```python
input("Enter your name: ")
```

**Q24: How do I store user input?**

```python
name = input("Enter name: ")
```

**Q25: How do I display two values?**

```python
print(name, score)
```

**Q26: How do I display text with a variable?**

```python
print(f"Hello {name}")
```

**Q27: How do I clear a console conceptually?**

```python
print("\n" * 50)
```

**Q28: How do I print multiple lines?**

```python
print("Line 1\nLine 2")
```

**Q29: How do I print a formatted message?**

```python
print(f"Score: {score}")
```

**Q30: How do I repeat output?**

```python
print("Hello" * 3)
```

</details>

<details>
<summary><h3>Basic Math Operations</h3></summary>

**Q31: How do I add two numbers?**

```python
result = a + b
```

**Q32: How do I subtract numbers?**

```python
result = a - b
```

**Q33: How do I multiply numbers?**

```python
result = a * b
```

**Q34: How do I divide numbers?**

```python
result = a / b
```

**Q35: How do I get the remainder?**

```python
result = a % b
```

**Q36: How do I increase a number by 1?**

```python
score += 1
```

**Q37: How do I decrease a number by 1?**

```python
score -= 1
```

**Q38: How do I double a value?**

```python
value *= 2
```

**Q39: How do I calculate an average?**

```python
avg = (a + b) / 2
```

**Q40: How do I square a number?**

```python
result = a * a
```

</details>

<details>
<summary><h3>Conditionals</h3></summary>

**Q41: How do I check if a number is greater than 10?**

```python
if number > 10:
    print("Big number")
```

**Q42: How do I check equality?**

```python
if a == b:
    print("Equal")
```

**Q43: How do I check if a number is even?**

```python
if number % 2 == 0:
    print("Even")
```

**Q44: How do I check if a number is odd?**

```python
if number % 2 != 0:
    print("Odd")
```

**Q45: How do I use else?**

```python
if age >= 18:
    print("Adult")
else:
    print("Minor")
```

**Q46: How do I check multiple conditions?**

```python
if age > 10 and age < 20:
    print("Teen")
```

**Q47: How do I use an or condition?**

```python
if a == 1 or a == 2:
    print("Match")
```

**Q48: How do I check if input is empty?**

```python
if name == "":
    print("Empty input")
```

**Q49: How do I check if a number is positive?**

```python
if number > 0:
    print("Positive")
```

**Q50: How do I nest conditions?**

```python
if age > 0:
    if age < 18:
        print("Minor")
```

</details>

<details>
<summary><h3>Random Numbers</h3></summary>

**Q51: How do I generate a random number from 1–10?**

```python
import random

random.randint(1, 10)
```

**Q52: How do I generate a random dice roll?**

```python
import random

random.randint(1, 6)
```

**Q53: How do I generate a random float?**

```python
import random

random.random()
```

**Q54: How do I pick random True/False?**

```python
import random

random.choice([True, False])
```

**Q55: How do I pick a random item from a list?**

```python
import random

random.choice(["A", "B", "C"])
```

**Q56: How do I simulate a coin flip?**

```python
import random

random.choice(["Heads", "Tails"])
```

**Q57: How do I generate a number between 50 and 100?**

```python
import random

random.randint(50, 100)
```

**Q58: How do I generate multiple random numbers?**

```python
import random

a = random.randint(1, 10)
b = random.randint(1, 10)
```

**Q59: How do I use randomness in a condition?**

```python
import random

if random.randint(1, 10) == 1:
    print("Lucky!")
```

**Q60: How do I run a random event in a CLI game?**

```python
import random

event = random.choice(["Fight", "Loot", "Nothing"])
print(event)
```

</details>

</details>

<details>
<summary><h2>Flowcharts for Sample Projects + Key</h2></summary>

<details>
<summary><h3>Flowchart Shape Key</h3></summary>

| Shape | Meaning |
| --- | --- |
| `([ START ])` | **Terminator** — Start/End |
| `[ Process ]` | **Rectangle** — Action/process |
| `[/ Input /]` | **Parallelogram** — User input/output |
| `{ Decision? }` | **Diamond** — Yes/No decision |
| `↓` | **Arrow** — Flow direction |

</details>

<details>
<summary><h3>PROJECT 1 — Number Guessing Game</h3></summary>

**Text Flowchart**

```text
        ([ START ])
             |
             ↓
   [ Generate random number
       between 1 and 10 ]
             |
             ↓
   [/ Ask user for a guess /]
             |
             ↓
      { Guess == Secret? }
          /          \
       YES            NO
        |              |
        ↓              ↓
[/ Print "You       [/ Print "Wrong!
   guessed it!" /]      The number was
                        [secret number]" /]
        |              |
        ↓              ↓
        └──────┬───────┘
               ↓
          ([ END ])
```

**Shape Breakdown**

1. **START** → Terminator
2. Generate random number → Process
3. Ask for guess → Input/Output
4. Compare guess to secret → Decision
5. Print "You guessed it!" → Input/Output
6. Print correct answer → Input/Output
7. **END** → Terminator

</details>

---

<details>
<summary><h3>PROJECT 2 — Simple Calculator</h3></summary>

**Text Flowchart**

```text
        ([ START ])
             |
             ↓
   [/ Get first number /]
             |
             ↓
  [/ Get second number /]
             |
             ↓
      [ Add num1 + num2
          → result ]
             |
             ↓
    [/ Display result /]
             |
             ↓
          ([ END ])
```

**Shape Breakdown**

1. **START** → Terminator
2. Get first number → Input/Output
3. Get second number → Input/Output
4. Add numbers → Process
5. Display result → Input/Output
6. **END** → Terminator

</details>

---

<details>
<summary><h3>PROJECT 3 — Even or Odd Checker</h3></summary>

**Text Flowchart**

```text
        ([ START ])
             |
             ↓
      [/ Get number /]
             |
             ↓
     { number % 2 == 0? }
          /         \
       YES           NO
        |             |
        ↓             ↓
 [/ Print "Even" /] [/ Print "Odd" /]
        |             |
        └──────┬──────┘
               ↓
          ([ END ])
```

**Shape Breakdown**

1. **START** → Terminator
2. Get number → Input/Output
3. Check `number % 2 == 0` → Decision
4. Print "Even" → Input/Output
5. Print "Odd" → Input/Output
6. **END** → Terminator

</details>

---

<details>
<summary><h3>PROJECT 4 — Mini Login System</h3></summary>

This one has a slightly more interesting decision because you're checking **two conditions at once**.

**Text Flowchart**

```text
        ([ START ])
             |
             ↓
   [ Set correct username
     and correct password ]
             |
             ↓
   [/ Ask for username /]
             |
             ↓
   [/ Ask for password /]
             |
             ↓
 { Username matches AND
   password matches? }
        /          \
      YES           NO
       |             |
       ↓             ↓
[/ Print "Login    [/ Print "Login
    successful" /]      failed" /]
       |             |
       └──────┬──────┘
              ↓
         ([ END ])
```

**Shape Breakdown**

1. **START** → Terminator
2. Set correct username/password → Process
3. Ask for username → Input/Output
4. Ask for password → Input/Output
5. Check both credentials → Decision
6. Print successful → Input/Output
7. Print failed → Input/Output
8. **END** → Terminator

**The Important Logic**

```text
Username correct?
       +
Password correct?
       ↓
      AND
       ↓
     Login?
```

So the diamond represents:

```text
username == correct_username
AND
password == correct_password
```

</details>

---

<details>
<summary><h3>PROJECT 5 — Dice Roll Game</h3></summary>

**Text Flowchart**

```text
        ([ START ])
             |
             ↓
    [ Generate random
       number 1-6 ]
             |
             ↓
    [/ Display dice roll /]
             |
             ↓
       { Dice == 6? }
          /       \
       YES         NO
        |           |
        ↓           ↓
[/ Print "Critical [/ Print "Try
     Roll!" /]         again!" /]
        |           |
        └─────┬─────┘
              ↓
         ([ END ])
```

**Shape Breakdown**

1. **START** → Terminator
2. Generate random dice number → Process
3. Display dice roll → Input/Output
4. Check `dice == 6` → Decision
5. Print "Critical Roll!" → Input/Output
6. Print "Try again!" → Input/Output
7. **END** → Terminator

</details>

</details>

<details>
<summary><h2>Sample Projects</h2></summary>

<details>
<summary><h3>PROJECT 1: Number Guessing Game</h3></summary>

```python
import random

# Step 1: Generate a random number between 1 and 10
secret_number = random.randint(1, 10)

# Step 2: Ask the user for a guess
guess = int(input("Guess a number (1-10): "))

# Step 3: Compare guess to secret number
if guess == secret_number:
    # Step 4: If correct, print win message
    print("You guessed it!")
else:
    # Step 5: If wrong, show correct answer
    print("Wrong! The number was", secret_number)
```

</details>

---

<details>
<summary><h3>PROJECT 2: Simple Calculator (Add Only)</h3></summary>

```python
# Step 1: Get first number from user
num1 = int(input("Enter first number: "))

# Step 2: Get second number from user
num2 = int(input("Enter second number: "))

# Step 3: Add numbers together
result = num1 + num2

# Step 4: Display result
print("Result:", result)
```

</details>

---

<details>
<summary><h3>PROJECT 3: Even or Odd Checker</h3></summary>

```python
# Step 1: Get number from user
number = int(input("Enter a number: "))

# Step 2: Check if number is even
if number % 2 == 0:
    # Step 3: Print even message
    print("Even")
else:
    # Step 4: Print odd message
    print("Odd")
```

</details>

---

<details>
<summary><h3>PROJECT 4: Mini Login System</h3></summary>

```python
# Step 1: Set correct username and password
correct_username = "admin"
correct_password = "1234"

# Step 2: Ask user for username
username = input("Username: ")

# Step 3: Ask user for password
password = input("Password: ")

# Step 4: Check if both match
if username == correct_username and password == correct_password:
    # Step 5: Success message
    print("Login successful")
else:
    # Step 6: Failure message
    print("Login failed")
```

</details>

---

<details>
<summary><h3>PROJECT 5: Dice Roll Game</h3></summary>

```python
import random

# Step 1: Roll a dice (1 to 6)
dice = random.randint(1, 6)

# Step 2: Show result
print("You rolled:", dice)

# Step 3: Check if user rolled the highest number
if dice == 6:
    # Step 4: Special message
    print("Critical Roll!")
else:
    # Step 5: Normal message
    print("Try again!")
```

</details>

</details>

</details>