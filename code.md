<details>

# Coding Basics/White Belt/Python + CLI

💡 Tip: Click the arrows next to each heading to expand or collapse the content underneath.

<summary><h2> # Key Concepts </h2></summary>

# Variables & Constants

### 1. What is a variable?

A variable is a box that stores information that can change.

### 2. When should I use a variable?

Use it when the value will change later (like score or health).

### 3. Why use a variable?

Because apps need to remember and update information.

### 4. How do I create a variable in Kotlin?

```kotlin
var score = 0
```

### 5. What is a constant?

A constant is a value that cannot change after it is set.

### 6. When should I use a constant?

When the value should stay the same (like app name).

### 7. Why use a constant?

To prevent accidental changes in important values.

### 8. How do I create a constant in Kotlin?

```kotlin
val appName = "MyApp"
```

### 9. What is the difference between var and val?

var = changeable, val = unchangeable.

### 10. Why is val preferred?

Because it makes code safer and easier to understand.

---

# Data Types

### 11. What is a data type?

A rule that tells Kotlin what kind of data something is.

### 12. What is an Int?

A whole number (like 1, 5, 100).

### 13. When do I use Int?

For counting, scores, and ages.

### 14. What is a String?

Text like words or sentences.

### 15. When do I use String?

For names, messages, or labels.

### 16. What is a Boolean?

A value that is only true or false.

### 17. When do I use Boolean?

For yes/no or on/off situations.

### 18. What is a Double?

A number with decimals.

### 19. When do I use Double?

For money or precise measurements.

### 20. Why are data types important?

They help prevent mistakes in calculations and logic.

---

# Input / Output

### 21. What is input?

Data the user gives to the app.

### 22. What is output?

Data the app shows to the user.

### 23. What is an EditText?

A box where the user types input.

### 24. When do I use EditText?

When I need user input like name or number.

### 25. What is a TextView?

A box that shows text output.

### 26. When do I use TextView?

When I want to display results.

### 27. How do I get text from EditText?

```kotlin
val name = editText.text.toString()
```

### 28. Why do we use `.toString()`?

Because EditText data must be converted into normal text.

### 29. How do I show text in TextView?

```kotlin
textView.text = "Hello"
```

### 30. Why is input/output important?

Because apps need to talk to the user.

---

# Basic Math Operations

### 31. What is basic math in programming?

Using code to calculate numbers.

### 32. What does + do?

Adds numbers together.

### 33. What does - do?

Subtracts numbers.

### 34. What does * do?

Multiplies numbers.

### 35. What does / do?

Divides numbers.

### 36. What does % do?

Gives the remainder after division.

### 37. When do I use %?

To check even or odd numbers.

### 38. What does ++ mean?

Increase a number by 1.

### 39. What does -- mean?

Decrease a number by 1.

### 40. Why is math used in apps?

For scores, money, physics, games, and logic.

---

# Conditionals (if / else)

### 41. What is a conditional?

A way for a program to make decisions.

### 42. What is an if statement?

Code that runs only if something is true.

### 43. When do I use if?

When I need different outcomes based on conditions.

### 44. What is else?

Code that runs when if is false.

### 45. When do I use else?

When I need a fallback option.

### 46. What does == mean?

Checks if two values are equal.

### 47. What does > mean?

Checks if something is bigger.

### 48. What does < mean?

Checks if something is smaller.

### 49. Why use conditionals?

To make apps respond differently to situations.

### 50. What happens without conditionals?

The app would always do the same thing.

---

# Random Numbers

### 51. What is a random number?

A number the computer picks unpredictably.

### 52. When do I use random numbers?

For games, dice, loot, or guessing.

### 53. Why use randomness?

To make apps feel more real and fun.

### 54. How do I generate a random number in Kotlin?

```kotlin
val num = (1..10).random()
```

### 55. How do I simulate a dice roll?

```kotlin
val roll = (1..6).random()
```

### 56. How do I generate a random Boolean?

```kotlin
val value = kotlin.random.Random.nextBoolean()
```

### 57. What is a range in Kotlin?

A set of numbers like 1..10.

### 58. Why use ranges?

They make random number limits easy.

### 59. How do I show a random number in TextView?

```kotlin
textView.text = (1..100).random().toString()
```

### 60. Why is randomness important in programming?

It adds unpredictability and makes apps more engaging.

```

```

<summary><h2> Code Syntax </h2></summary>

# Variables & Constants

Q1:
How do I create a variable that stores a player's score?

```python
score = 0
```

Q2:
How do I create a constant for an app name?

```python
APP_NAME = "My CLI App"
```

Q3:
How do I store a user's name?

```python
name = "John"
```

Q4:
How do I update a score variable?

```python
score = score + 1
```

Q5:
How do I reset a variable to zero?

```python
score = 0
```

Q6:
How do I copy one variable into another?

```python
backup = score
```

Q7:
How do I store a game status as a variable?

```python
is_running = True
```

Q8:
How do I change a variable based on condition later?

```python
score = score + 10
```

Q9:
How do I store a message in a variable?

```python
message = "Hello Player"
```

Q10:
How do I define a constant for max score?

```python
MAX_SCORE = 100
```

# Data Types

Q11:
How do I store an integer number?

```python
age = 25
```

Q12:
How do I store a decimal number?

```python
price = 9.99
```

Q13:
How do I store text?

```python
name = "Alice"
```

Q14:
How do I store a true/false value?

```python
is_alive = True
```

Q15:
How do I convert input into an integer?

```python
number = int(input())
```

Q16:
How do I convert input into a float?

```python
number = float(input())
```

Q17:
How do I store multiple words in a string?

```python
message = "Hello World"
```

Q18:
How do I check a variable type?

```python
type(score)
```

Q19:
How do I store a negative number?

```python
value = -5
```

Q20:
How do I convert number to string?

```python
str(score)
```

# Input / Output

Q21:
How do I print a message?

```python
print("Hello World")
```

Q22:
How do I print a variable?

```python
print(score)
```

Q23:
How do I get user input?

```python
input("Enter your name: ")
```

Q24:
How do I store user input?

```python
name = input("Enter name: ")
```

Q25:
How do I display two values?

```python
print(name, score)
```

Q26:
How do I display text with a variable?

```python
print(f"Hello {name}")
```

Q27:
How do I clear a console (conceptually)?

```python
print("\n" * 50)
```

Q28:
How do I print multiple lines?

```python
print("Line 1\nLine 2")
```

Q29:
How do I print a formatted message?

```python
print(f"Score: {score}")
```

Q30:
How do I repeat output?

```python
print("Hello" * 3)
```

# Basic Math Operations

Q31:
How do I add two numbers?

```python
result = a + b
```

Q32:
How do I subtract numbers?

```python
result = a - b
```

Q33:
How do I multiply numbers?

```python
result = a * b
```

Q34:
How do I divide numbers?

```python
result = a / b
```

Q35:
How do I get remainder?

```python
result = a % b
```

Q36:
How do I increase a number by 1?

```python
score += 1
```

Q37:
How do I decrease a number by 1?

```python
score -= 1
```

Q38:
How do I double a value?

```python
value *= 2
```

Q39:
How do I calculate average?

```python
avg = (a + b) / 2
```

Q40:
How do I square a number?

```python
result = a * a
```

# Conditionals

Q41:
How do I check if a number is greater than 10?

```python
if number > 10:
    print("Big number")
```

Q42:
How do I check equality?

```python
if a == b:
    print("Equal")
```

Q43:
How do I check if a number is even?

```python
if number % 2 == 0:
    print("Even")
```

Q44:
How do I check if a number is odd?

```python
if number % 2 != 0:
    print("Odd")
```

Q45:
How do I use else?

```python
if age >= 18:
    print("Adult")
else:
    print("Minor")
```

Q46:
How do I check multiple conditions?

```python
if age > 10 and age < 20:
    print("Teen")
```

Q47:
How do I use or condition?

```python
if a == 1 or a == 2:
    print("Match")
```

Q48:
How do I check if input is empty?

```python
if name == "":
    print("Empty input")
```

Q49:
How do I check if a number is positive?

```python
if number > 0:
    print("Positive")
```

Q50:
How do I nest conditions?

```python
if age > 0:
    if age < 18:
        print("Minor")
```

# Random Numbers

Q51:
How do I generate a random number 1–10?

```python
import random
random.randint(1, 10)
```

Q52:
How do I generate a random dice roll?

```python
import random
random.randint(1, 6)
```

Q53:
How do I generate a random float?

```python
import random
random.random()
```

Q54:
How do I pick random True/False?

```python
import random
random.choice([True, False])
```

Q55:
How do I pick a random item from a list?

```python
import random
random.choice(["A", "B", "C"])
```

Q56:
How do I simulate coin flip?

```python
import random
random.choice(["Heads", "Tails"])
```

Q57:
How do I generate a number between 50 and 100?

```python
import random
random.randint(50, 100)
```

Q58:
How do I generate multiple random numbers?

```python
import random
a = random.randint(1, 10)
b = random.randint(1, 10)
```

Q59:
How do I use randomness in a condition?

```python
import random
if random.randint(1, 10) == 1:
    print("Lucky!")
```

Q60:
How do I run a random event in CLI game?

```python
import random
event = random.choice(["Fight", "Loot", "Nothing"])
print(event)
```

<summary><h2> Flowcharts for Sample Projects + Key</h2></summary>

### Flowchart shape key

| Shape | Meaning |
| --- | --- |
| `([ START ])` | **Terminator** — Start/End |
| `[ Process ]` | **Rectangle** — Action/process |
| `[/ Input /]` | **Parallelogram** — User input/output |
| `{ Decision? }` | **Diamond** — Yes/No decision |
| `↓` | **Arrow** — Flow direction |

# PROJECT 1 — Number Guessing Game

### Text Flowchart

```
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
[/ Print "You      [/ Print "Wrong!
   guessed it!" /]      The number was
                        [secret number]" /]
        |              |
        ↓              ↓
        └──────┬───────┘
               ↓
          ([ END ])
```

### Shape breakdown

1. **START** → Terminator
2. Generate random number → Process
3. Ask for guess → Input/Output
4. Compare guess to secret → Decision
5. Print "You guessed it!" → Input/Output
6. Print correct answer → Input/Output
7. **END** → Terminator

---

# PROJECT 2 — Simple Calculator

### Text Flowchart

```
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

### Shape breakdown

1. **START** → Terminator
2. Get first number → Input/Output
3. Get second number → Input/Output
4. Add numbers → Process
5. Display result → Input/Output
6. **END** → Terminator

---

# PROJECT 3 — Even or Odd Checker

### Text Flowchart

```
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

### Shape breakdown

1. **START** → Terminator
2. Get number → Input/Output
3. Check `number % 2 == 0` → Decision
4. Print "Even" → Input/Output
5. Print "Odd" → Input/Output
6. **END** → Terminator

---

# PROJECT 4 — Mini Login System

This one has a slightly more interesting decision because you're checking **two conditions at once**.

### Text Flowchart

```
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

### Shape breakdown

1. **START** → Terminator
2. Set correct username/password → Process
3. Ask for username → Input/Output
4. Ask for password → Input/Output
5. Check both credentials → Decision
6. Print successful → Input/Output
7. Print failed → Input/Output
8. **END** → Terminator

### The important logic

```
Username correct?
       +
Password correct?
       ↓
     AND
       ↓
   Login?
```

So the diamond represents:

```
username == correct_username
AND
password == correct_password
```

---

# PROJECT 5 — Dice Roll Game

### Text Flowchart

```
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

### Shape breakdown

1. **START** → Terminator
2. Generate random dice number → Process
3. Display dice roll → Input/Output
4. Check `dice == 6` → Decision
5. Print "Critical Roll!" → Input/Output
6. Print "Try again!" → Input/Output
7. **END** → Terminator

<summary><h2> Sample Projects </h2></summary>

# PROJECT 1: Number Guessing Game

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

---

# PROJECT 2: Simple Calculator (Add Only)

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

---

# PROJECT 3: Even or Odd Checker

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

---

# PROJECT 4: Mini Login System

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

---

# PROJECT 5: Dice Roll Game

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
