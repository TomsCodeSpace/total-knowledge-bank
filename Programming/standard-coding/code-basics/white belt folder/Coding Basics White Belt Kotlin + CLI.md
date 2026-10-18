<details>
<summary><h1>Coding Basics/White Belt/Kotlin + CLI</h1></summary>

💡 Tip: Click the arrows next to each heading to expand or collapse the content underneath.

<details>
<summary><h2>Key Concepts</h2></summary>

<details>
<summary><h3>Variables and Constants</h3></summary>

Q1: What is a variable?

A: A variable is a labeled box that stores information you can change later.

Q2: When should I use a variable?

A: Use a variable when the value might change while your program runs.

Q3: What is a constant?

A: A constant is a labeled box whose value cannot change after it is created.

Q4: When should I use a constant?

A: Use a constant for values that should always stay the same, like PI or a tax rate.

Q5: Why use constants instead of variables?

A: They prevent accidental changes and make code safer.

Q6: How do I create a variable?

A:

```kotlin
var score = 0
```

Q7: How do I create a constant?

A:

```kotlin
val maxLives = 3
```

Q8: What is the difference between var and val?

A: var can change. val cannot.

Q9: Can I change a val?

A: No. Once assigned, its value stays the same.

Q10: Should I use val or var by default?

A: Use val unless you know the value needs to change.

</details>

<details>
<summary><h3>Data Types</h3></summary>

Q11: What is a data type?

A: A data type tells Kotlin what kind of information is stored.

Q12: What is an Int?

A: An Int stores whole numbers.

Q13: What is a Double?

A: A Double stores numbers with decimal places.

Q14: What is a String?

A: A String stores text.

Q15: What is a Boolean?

A: A Boolean stores either true or false.

Q16: When should I use an Int?

A: Use it for counting things like lives or scores.

Q17: When should I use a Double?

A: Use it when decimals matter, like money or measurements.

Q18: When should I use a String?

A: Use it for names, messages, and sentences.

Q19: When should I use a Boolean?

A: Use it when something has only two states, like on/off.

Q20: How do I create variables of different types?

A:

```kotlin
val age = 25
val height = 5.9
val name = "Alex"
val online = true
```

</details>

<details>
<summary><h3>Input and Output</h3></summary>

Q21: What is output?

A: Output is information your program shows to the user.

Q22: How do I print text?

A:

```kotlin
println("Hello!")
```

Q23: What is println()?

A: It prints text and moves to the next line.

Q24: What is print()?

A: It prints text without moving to the next line.

Q25: What is input?

A: Input is information the user gives the program.

Q26: How do I read user input?

A:

```kotlin
val name = readln()
```

Q27: Why do I need input?

A: It lets the user interact with your program.

Q28: How do I ask the user a question?

A:

```kotlin
print("Enter your name: ")
val name = readln()
```

Q29: How do I print a variable?

A:

```kotlin
val score = 100
println(score)
```

Q30: How do I combine text and variables?

A:

```kotlin
val name = "Alex"
println("Hello, $name")
```

</details>

<details>
<summary><h3>Basic Math Operations</h3></summary>

Q31: Why can Kotlin do math?

A: It has built-in math operators just like a calculator.

Q32: How do I add numbers?

A:

```kotlin
val total = 5 + 3
```

Q33: How do I subtract numbers?

A:

```kotlin
val total = 10 - 4
```

Q34: How do I multiply numbers?

A:

```kotlin
val total = 6 * 7
```

Q35: How do I divide numbers?

A:

```kotlin
val total = 20 / 5
```

Q36: What does % do?

A: It gives the remainder after division.

Q37: When is % useful?

A: To check if a number is even or odd.

Q38: How do I increase a variable?

A:

```kotlin
score++
```

Q39: How do I decrease a variable?

A:

```kotlin
score--
```

Q40: Why store math results in variables?

A: So you can reuse the answer later.

</details>

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

Q41: What is an if statement?

A: It lets your program make decisions.

Q42: When should I use if?

A: When different situations need different actions.

Q43: How do I check if something is true?

A:

```kotlin
if (score > 50) {
    println("You win!")
}
```

Q44: What does else do?

A: It runs if the if condition is false.

Q45: Why use else?

A: So every situation has a response.

Q46: What is else if?

A: It checks another condition if the first one fails.

Q47: How do I compare two values?

A:

```kotlin
if (age == 18)
```

Q48: What are common comparison operators?

A: ==, !=, <, >, <=, >=

Q49: What happens if the condition is false?

A: Kotlin skips that block of code.

Q50: Why are conditionals important?

A: They let programs react to different situations.

</details>

<details>
<summary><h3>Random Numbers</h3></summary>

Q51: What is a random number?

A: A number chosen unpredictably by the computer.

Q52: When should I use random numbers?

A: For games, simulations, and choosing random items.

Q53: Why use randomness?

A: It makes programs less predictable.

Q54: How do I generate a random number?

A:

```kotlin
import kotlin.random.Random

val number = Random.nextInt(1, 11)
```

Q55: What does Random.nextInt(1, 11) do?

A: It picks a random number from 1 through 10.

Q56: How do I simulate a coin flip?

A:

```kotlin
val coin = Random.nextInt(2)
```

Q57: How do I simulate a six-sided die?

A:

```kotlin
val roll = Random.nextInt(1, 7)
```

Q58: Can I use random numbers in if statements?

A: Yes. They work great together.

Q59: What kinds of programs use random numbers?

A: Games, quizzes, lotteries, AI, and simulations.

Q60: What is a simple random number game?

A:

```kotlin
import kotlin.random.Random

val secret = Random.nextInt(1, 11)

print("Guess a number (1-10): ")
val guess = readln().toInt()

if (guess == secret) {
    println("Correct!")
} else {
    println("Wrong! The number was $secret")
}
```

</details>
</details>

<details>
<summary><h2>Code Syntax</h2></summary>

<details>
<summary><h3>Variables and Constants</h3></summary>

Q1: Add a variable to store the player's score.

```kotlin
var score = 0
```

Q2: Add a constant for the maximum number of lives.

```kotlin
val MAX_LIVES = 3
```

Q3: Add a variable to store the player's name.

```kotlin
var playerName = "Unknown"
```

Q4: Add a variable to track whether the game is running.

```kotlin
var gameRunning = true
```

Q5: Add a constant for the game's title.

```kotlin
val GAME_TITLE = "Adventure Quest"
```

Q6: Add a variable to store the player's level.

```kotlin
var level = 1
```

Q7: Add a variable to store today's temperature.

```kotlin
var temperature = 72.5
```

Q8: Add a variable to store whether music is enabled.

```kotlin
var musicEnabled = true
```

Q9: Add a variable to store the user's age.

```kotlin
var age = 18
```

Q10: Add a constant for the speed of light.

```kotlin
val SPEED_OF_LIGHT = 299792458
```

</details>

<details>
<summary><h3>Data Types</h3></summary>

Q11: Add an Int variable for a player's health.

```kotlin
var health: Int = 100
```

Q12: Add a Double variable for a bank balance.

```kotlin
var balance: Double = 150.75
```

Q13: Add a String variable for a city name.

```kotlin
var city: String = "Dallas"
```

Q14: Add a Boolean variable to track login status.

```kotlin
var loggedIn: Boolean = false
```

Q15: Add a String for a password.

```kotlin
var password = "abc123"
```

Q16: Add an Int variable for an inventory count.

```kotlin
var inventory = 12
```

Q17: Add a Double variable for fuel remaining.

```kotlin
var fuel = 42.8
```

Q18: Add a Boolean indicating if the player has a key.

```kotlin
var hasKey = false
```

Q19: Add a String variable for an email address.

```kotlin
var email = "user@example.com"
```

Q20: Add an Int variable for a timer.

```kotlin
var timer = 60
```

</details>

<details>
<summary><h3>Input and Output</h3></summary>

Q21: Print "Hello, World!".

```kotlin
println("Hello, World!")
```

Q22: Ask the user for their name.

```kotlin
print("Enter your name: ")
val name = readln()
```

Q23: Print the user's name.

```kotlin
println(name)
```

Q24: Ask the user for their age.

```kotlin
print("Enter your age: ")
val age = readln().toInt()
```

Q25: Print a welcome message with the user's name.

```kotlin
println("Welcome, $name!")
```

Q26: Print two blank lines.

```kotlin
println()
println()
```

Q27: Print a menu.

```kotlin
println("1. Start")
println("2. Options")
println("3. Exit")
```

Q28: Ask the user for a decimal number.

```kotlin
print("Enter a decimal number: ")
val number = readln().toDouble()
```

Q29: Print multiple variables.

```kotlin
println("Name: $name")
println("Age: $age")
```

Q30: Prompt the user before reading input.

```kotlin
print("Enter anything: ")
val input = readln()
```

</details>

<details>
<summary><h3>Basic Math Operations</h3></summary>

Q31: Add two numbers together.

```kotlin
val sum = 8 + 4
```

Q32: Subtract two numbers.

```kotlin
val difference = 20 - 5
```

Q33: Multiply two numbers.

```kotlin
val product = 7 * 9
```

Q34: Divide two numbers.

```kotlin
val quotient = 50 / 5
```

Q35: Find the remainder after division.

```kotlin
val remainder = 17 % 5
```

Q36: Increase a score by one.

```kotlin
score++
```

Q37: Decrease the number of lives.

```kotlin
lives--
```

Q38: Add 10 points to the score.

```kotlin
score += 10
```

Q39: Double the player's money.

```kotlin
money *= 2
```

Q40: Calculate the average of two numbers.

```kotlin
val average = (a + b) / 2.0
```

</details>

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

Q41: Print "Winner!" if the score is above 100.

```kotlin
if (score > 100) {
    println("Winner!")
}
```

Q42: Print whether someone is an adult.

```kotlin
if (age >= 18) {
    println("Adult")
} else {
    println("Minor")
}
```

Q43: Check if a password is correct.

```kotlin
if (password == "secret") {
    println("Access Granted")
}
```

Q44: Check if the player has a key.

```kotlin
if (hasKey) {
    println("Door unlocked.")
}
```

Q45: Print if a number is positive.

```kotlin
if (number > 0) {
    println("Positive")
}
```

Q46: Check if a number is even.

```kotlin
if (number % 2 == 0) {
    println("Even")
}
```

Q47: Print a warning if health is low.

```kotlin
if (health < 25) {
    println("Low Health!")
}
```

Q48: Print "Correct" or "Incorrect".

```kotlin
if (guess == answer) {
    println("Correct")
} else {
    println("Incorrect")
}
```

Q49: Check whether someone can vote.

```kotlin
if (age >= 18) {
    println("Can Vote")
}
```

Q50: Choose between three grades.

```kotlin
if (grade >= 90) {
    println("A")
} else if (grade >= 80) {
    println("B")
} else {
    println("C or Below")
}
```

</details>

<details>
<summary><h3>Random Numbers</h3></summary>

Q51: Generate a random number from 1 to 10.

```kotlin
import kotlin.random.Random

val number = Random.nextInt(1, 11)
```

Q52: Simulate rolling a six-sided die.

```kotlin
import kotlin.random.Random

val roll = Random.nextInt(1, 7)
```

Q53: Simulate flipping a coin.

```kotlin
import kotlin.random.Random

val coin = Random.nextInt(2)
```

Q54: Pick a random number from 100 to 999.

```kotlin
import kotlin.random.Random

val code = Random.nextInt(100, 1000)
```

Q55: Generate a random health bonus.

```kotlin
import kotlin.random.Random

val bonus = Random.nextInt(5, 21)
```

Q56: Generate a random damage amount.

```kotlin
import kotlin.random.Random

val damage = Random.nextInt(10, 51)
```

Q57: Randomly choose between two outcomes.

```kotlin
import kotlin.random.Random

if (Random.nextBoolean()) {
    println("Heads")
} else {
    println("Tails")
}
```

Q58: Print a random number every time the program starts.

```kotlin
import kotlin.random.Random

println(Random.nextInt(1, 101))
```

Q59: Give the player a random amount of gold.

```kotlin
import kotlin.random.Random

val gold = Random.nextInt(50, 201)
```

Q60: Create a random guessing game.

```kotlin
import kotlin.random.Random

val secret = Random.nextInt(1, 11)

print("Guess (1-10): ")
val guess = readln().toInt()

if (guess == secret) {
    println("Correct!")
} else {
    println("Wrong! The answer was $secret")
}
```

</details>
</details>

<details>
<summary><h2>Flowcharts + Key</h2></summary>

<details>
<summary><h3>Flowchart Shape Key</h3></summary>

| Shape | Meaning | Kotlin examples |
| --- | --- | --- |
| `([ START / END ])` | **Oval / Terminator** | Program start/end |
| `[ Process ]` | **Rectangle** | Variables, calculations, random generation |
| `[/ Input / Output /]` | **Parallelogram** | `readln()`, `print()`, `println()` |
| `{ Condition? }` | **Diamond** | `if`, `when`, comparisons |
| `↓` | **Arrow** | Program flow |

</details>

<details>
<summary><h3>Project 1: Number Guessing Game</h3></summary>

<details>
<summary><h4>Text-Based Flowchart</h4></summary>

```
([ START ])
     ↓
[ Import Random library ]
     ↓
[ Generate secret number from 1–10 ]
     ↓
[/ Display "Guess a number (1-10):" /]
     ↓
[/ Read user input /]
     ↓
[ Convert input to Int ]
     ↓
[ Store input as guess ]
     ↓
{ guess == secret? }
       ↙          ↘
     YES           NO
      ↓             ↓
[/ Display      [/ Display
  "Correct!" /]   "Wrong! The number
                  was secret" /]
       ↘          ↙
          ↓
      ([ END ])
```

</details>

<details>
<summary><h4>Flowchart Shapes</h4></summary>

- **START** → Oval
- **Import Random library** → Rectangle
- **Generate secret number** → Rectangle
- **Display guess prompt** → Parallelogram
- **Read input** → Parallelogram
- **Convert to Int** → Rectangle
- **Store as `guess`** → Rectangle
- **`guess == secret?`** → Diamond
- **Display Correct** → Parallelogram
- **Display Wrong** → Parallelogram
- **END** → Oval

</details>

<details>
<summary><h4>Core Pattern</h4></summary>

```
GENERATE
   ↓
INPUT
   ↓
CONVERT
   ↓
COMPARE
 ↙     ↘
YES    NO
 ↓      ↓
OUTPUT OUTPUT
   ↘   ↙
    END
```

</details>
</details>

<details>
<summary><h3>Project 2: Simple Calculator</h3></summary>

This one uses a `when` statement, so the flowchart is essentially a **multi-way decision**.

<details>
<summary><h4>Text-Based Flowchart</h4></summary>

```
([ START ])
     ↓
[/ Ask for first number /]
     ↓
[/ Read input /]
     ↓
[ Convert to Double ]
     ↓
[ Store as num1 ]
     ↓
[/ Ask for second number /]
     ↓
[/ Read input /]
     ↓
[ Convert to Double ]
     ↓
[ Store as num2 ]
     ↓
[/ Ask for operation (+, -, *, /) /]
     ↓
[/ Read operation /]
     ↓
[ Store as op ]
     ↓
{ Which operation? }
   ↙      ↓       ↓       ↘
  "+"     "-"     "*"      "/"
   ↓       ↓       ↓        ↓
[ num1   [ num1   [ num1    [ num1
  + num2 ]  - num2 ]  * num2 ]  / num2 ]
   ↘       ↓       ↓        ↙
      ↘    ↓       ↓      ↙
          [ result ]
              ↑
              │
           "else"
              ↓
      [/ Display "Invalid
          operation" /]
              ↓
        [ result = 0.0 ]
              ↓
              └──────────┐
                         ↓
              [/ Display result /]
                         ↓
                     ([ END ])
```

</details>

<details>
<summary><h4>Cleaner Conceptual Version</h4></summary>

```
                { op? }
          ↙       ↓       ↓       ↘
        "+"      "-"      "*"      "/"
         ↓        ↓        ↓        ↓
       ADD      SUBTRACT MULTIPLY DIVIDE
          ↘       ↓       ↓       ↙
                  ↓
              [ result ]
                  ↑
                  │
               "else"
                  ↓
          [/ Invalid operation /]
                  ↓
             [ result = 0 ]
                  ↓
                  └──────→ [ result ]
                               ↓
                          [/ Output /]
                               ↓
                            ([ END ])
```

</details>

<details>
<summary><h4>Flowchart Shapes</h4></summary>

- **START** → Oval
- **Ask for numbers/operation** → Parallelogram
- **Read input** → Parallelogram
- **Convert to Double** → Rectangle
- **Store `num1`, `num2`, `op`** → Rectangles
- **`Which operation?`** → Diamond
- **Addition** → Rectangle
- **Subtraction** → Rectangle
- **Multiplication** → Rectangle
- **Division** → Rectangle
- **Invalid operation** → Parallelogram
- **`result = 0.0`** → Rectangle
- **Display result** → Parallelogram
- **END** → Oval

</details>

<details>
<summary><h4>Core Pattern</h4></summary>

```
INPUT
  ↓
CONVERT
  ↓
STORE
  ↓
{ OPERATION? }
 ↙   ↓   ↓   ↘
+    -   *    /
↓    ↓   ↓    ↓
ADD SUB MUL DIV
 ↘   ↓   ↓   ↙
    RESULT
       ↓
    OUTPUT
       ↓
      END
```

</details>
</details>

<details>
<summary><h3>Project 3: Health Battle Simulator</h3></summary>

There aren't actually any decision branches in this version. It is a straight sequence of calculations.

<details>
<summary><h4>Text-Based Flowchart</h4></summary>

```
([ START ])
     ↓
[ Import Random library ]
     ↓
[ Set playerHealth = 100 ]
     ↓
[ Set enemyHealth = 100 ]
     ↓
[ Generate playerDamage from 10–30 ]
     ↓
[ Subtract playerDamage from enemyHealth ]
     ↓
[ Generate enemyDamage from 5–20 ]
     ↓
[ Subtract enemyDamage from playerHealth ]
     ↓
[/ Display player damage /]
     ↓
[/ Display enemy damage /]
     ↓
[/ Display Player Health /]
     ↓
[/ Display Enemy Health /]
     ↓
([ END ])
```

</details>

<details>
<summary><h4>Flowchart Shapes</h4></summary>

- **START** → Oval
- **Import Random** → Rectangle
- **Set player health** → Rectangle
- **Set enemy health** → Rectangle
- **Generate player damage** → Rectangle
- **Subtract damage from enemy** → Rectangle
- **Generate enemy damage** → Rectangle
- **Subtract damage from player** → Rectangle
- **Display damage values** → Parallelograms
- **Display health values** → Parallelograms
- **END** → Oval

</details>

<details>
<summary><h4>Core Pattern</h4></summary>

```
SETUP
  ↓
RANDOM DAMAGE
  ↓
MODIFY ENEMY
  ↓
RANDOM DAMAGE
  ↓
MODIFY PLAYER
  ↓
OUTPUT
  ↓
END
```

**Important:** There is no `{ Condition? }` diamond because the code never checks whether someone is dead or whether one player won.

</details>
</details>

<details>
<summary><h3>Project 4: Login System</h3></summary>

<details>
<summary><h4>Text-Based Flowchart</h4></summary>

```
([ START ])
     ↓
[ Store correctUsername = "admin" ]
     ↓
[ Store correctPassword = "1234" ]
     ↓
[/ Display "Enter username:" /]
     ↓
[/ Read username /]
     ↓
[/ Display "Enter password:" /]
     ↓
[/ Read password /]
     ↓
{ username == correctUsername
  AND
  password == correctPassword? }
       ↙                  ↘
     YES                   NO
      ↓                     ↓
[/ Display              [/ Display
  "Access                 "Access
  Granted" /]              Denied" /]
       ↘                  ↙
           ↓
       ([ END ])
```

</details>

<details>
<summary><h4>Flowchart Shapes</h4></summary>

- **START** → Oval
- **Store credentials** → Rectangles
- **Display username prompt** → Parallelogram
- **Read username** → Parallelogram
- **Display password prompt** → Parallelogram
- **Read password** → Parallelogram
- **Credentials correct?** → Diamond
- **Access Granted** → Parallelogram
- **Access Denied** → Parallelogram
- **END** → Oval

</details>

<details>
<summary><h4>Core Logic</h4></summary>

```
username correct ──┐
                   ├── AND ──→ { Valid credentials? }
password correct ──┘
                              ↙       ↘
                            YES       NO
                             ↓         ↓
                          GRANTED    DENIED
```

Both conditions have to be true.

</details>
</details>

<details>
<summary><h3>Project 5: Random Loot Box System</h3></summary>

This one is another `when`-based **multi-way decision**.

<details>
<summary><h4>Text-Based Flowchart</h4></summary>

```
([ START ])
     ↓
[ Define item1 = "Wooden Sword" ]
     ↓
[ Define item2 = "Iron Sword" ]
     ↓
[ Define item3 = "Golden Sword" ]
     ↓
[ Generate random roll from 1–3 ]
     ↓
[ Store roll ]
     ↓
{ What is roll? }
    ↙       ↓       ↘
   1        2        3
   ↓        ↓        ↓
[ loot =  [ loot =  [ loot =
  item1 ]   item2 ]   item3 ]
    ↘        ↓        ↙
       ↘    ↓     ↙
          [ loot ]
             ↑
             │
          "else"
             ↓
      [ loot = "Nothing" ]
             ↓
             └─────────┐
                       ↓
            [/ Display "You opened
                a loot box..." /]
                       ↓
            [/ Display received loot /]
                       ↓
                   ([ END ])
```

</details>

<details>
<summary><h4>Cleaner Conceptual Version</h4></summary>

```
          [ RANDOM ROLL 1–3 ]
                  ↓
             { roll? }
           ↙     ↓     ↘
          1      2      3
          ↓      ↓      ↓
       WOODEN   IRON   GOLDEN
       SWORD   SWORD   SWORD
          ↘      ↓      ↙
             [ LOOT ]
                ↓
             OUTPUT
                ↓
               END
```

</details>

<details>
<summary><h4>Flowchart Shapes</h4></summary>

- **START** → Oval
- **Define loot items** → Rectangles
- **Generate random roll** → Rectangle
- **Store roll** → Rectangle
- **`What is roll?`** → Diamond
- **Select item 1** → Rectangle
- **Select item 2** → Rectangle
- **Select item 3** → Rectangle
- **Fallback `"Nothing"`** → Rectangle
- **Display loot-box message** → Parallelogram
- **Display received item** → Parallelogram
- **END** → Oval

</details>
</details>

<details>
<summary><h3>Kotlin CLI Master Flowchart</h3></summary>

These five give you a nice progression because they introduce several different control-flow patterns:

```
                    ([ START ])
                         ↓
                    [ SETUP ]
                         ↓
                      INPUT
                         ↓
                    [ PROCESS ]
                         ↓
                 { DECISION? }
                  ↙         ↘
                YES          NO
                 ↓            ↓
            [ PROCESS ]  [ PROCESS ]
                  ↘         ↙
                     ↓
                   OUTPUT
                     ↓
                  ([ END ])
```

But there are actually **three important flow patterns** represented by your projects.

<details>
<summary><h4>1. Straight-line sequence — Health Battle</h4></summary>

```
START
 ↓
PROCESS
 ↓
PROCESS
 ↓
PROCESS
 ↓
OUTPUT
 ↓
END
```

</details>

<details>
<summary><h4>2. Binary decision — Number Guessing / Login</h4></summary>

```
       { CONDITION? }
         ↙       ↘
       YES       NO
        ↓         ↓
     OUTPUT     OUTPUT
         ↘     ↙
           END
```

</details>

<details>
<summary><h4>3. Multi-way decision — Calculator / Loot Box</h4></summary>

```
            { VALUE? }
          ↙    ↓    ↘
        CASE  CASE  CASE
          ↓    ↓    ↓
       PROCESS PROCESS PROCESS
          ↘    ↓    ↙
            OUTPUT
               ↓
              END
```

</details>
</details>
</details>

<details>
<summary><h2>Sample Projects</h2></summary>

<details>
<summary><h3>Project 1: Number Guessing Game</h3></summary>

<details>
<summary><h4>Steps</h4></summary>

1. Generate a random number
2. Ask user to guess
3. Read input
4. Compare guess
5. Print result

</details>

```kotlin
import kotlin.random.Random

fun main() {

    // STEP 1: Generate a secret random number between 1 and 10
    val secret = Random.nextInt(1, 11)

    // STEP 2: Ask the user for a guess
    print("Guess a number (1-10): ")

    // STEP 3: Read user input and convert to Int
    val guess = readln().toInt()

    // STEP 4: Compare guess to secret number
    if (guess == secret) {

        // STEP 5A: Correct guess
        println("Correct!")
    } else {

        // STEP 5B: Wrong guess
        println("Wrong! The number was $secret")
    }
}
```

</details>

<details>
<summary><h3>Project 2: Simple Calculator</h3></summary>

<details>
<summary><h4>Steps</h4></summary>

1. Ask for first number
2. Ask for second number
3. Ask for operation
4. Perform calculation
5. Print result

</details>

```kotlin
fun main() {

    // STEP 1: Get first number
    print("Enter first number: ")
    val num1 = readln().toDouble()

    // STEP 2: Get second number
    print("Enter second number: ")
    val num2 = readln().toDouble()

    // STEP 3: Get operation (+, -, *, /)
    print("Enter operation (+, -, *, /): ")
    val op = readln()

    // STEP 4: Perform calculation based on operation
    val result = when (op) {

        "+" -> num1 + num2
        "-" -> num1 - num2
        "*" -> num1 * num2
        "/" -> num1 / num2

        // Default case if invalid input
        else -> {
            println("Invalid operation")
            0.0
        }
    }

    // STEP 5: Print result
    println("Result: $result")
}
```

</details>

<details>
<summary><h3>Project 3: Health Battle Simulator</h3></summary>

<details>
<summary><h4>Steps</h4></summary>

1. Set player and enemy health
2. Generate random damage
3. Player attacks enemy
4. Enemy attacks player
5. Print final health

</details>

```kotlin
import kotlin.random.Random

fun main() {

    // STEP 1: Set starting health values
    var playerHealth = 100
    var enemyHealth = 100

    // STEP 2: Player attacks first (random damage)
    val playerDamage = Random.nextInt(10, 31)
    enemyHealth -= playerDamage

    // STEP 3: Enemy attacks back (random damage)
    val enemyDamage = Random.nextInt(5, 21)
    playerHealth -= enemyDamage

    // STEP 4: Print damage results
    println("Player dealt $playerDamage damage")
    println("Enemy dealt $enemyDamage damage")

    // STEP 5: Print final health values
    println("Player Health: $playerHealth")
    println("Enemy Health: $enemyHealth")
}
```

</details>

<details>
<summary><h3>Project 4: Login System (Basic CLI)</h3></summary>

<details>
<summary><h4>Steps</h4></summary>

1. Store correct username/password
2. Ask user for username
3. Ask user for password
4. Compare values
5. Print access result

</details>

```kotlin
fun main() {

    // STEP 1: Stored credentials
    val correctUsername = "admin"
    val correctPassword = "1234"

    // STEP 2: Ask for username
    print("Enter username: ")
    val username = readln()

    // STEP 3: Ask for password
    print("Enter password: ")
    val password = readln()

    // STEP 4: Check credentials
    if (username == correctUsername && password == correctPassword) {

        // STEP 5A: Successful login
        println("Access Granted")
    } else {

        // STEP 5B: Failed login
        println("Access Denied")
    }
}
```

</details>

<details>
<summary><h3>Project 5: Random Loot Box System</h3></summary>

<details>
<summary><h4>Steps</h4></summary>

1. Define possible loot items
2. Generate random selection
3. Pick item based on random number
4. Assign item to player
5. Print result

</details>

```kotlin
import kotlin.random.Random

fun main() {

    // STEP 1: Define loot items (simple pool)
    val item1 = "Wooden Sword"
    val item2 = "Iron Sword"
    val item3 = "Golden Sword"

    // STEP 2: Generate random number
    val roll = Random.nextInt(1, 4)

    // STEP 3: Choose item based on roll
    val loot = when (roll) {

        1 -> item1
        2 -> item2
        3 -> item3

        // fallback (should never happen)
        else -> "Nothing"
    }

    // STEP 4: Assign loot to player (conceptual)
    println("You opened a loot box...")

    // STEP 5: Print result
    println("You received: $loot")
}
```

</details>
</details>

</details>