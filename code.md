
<details>

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
