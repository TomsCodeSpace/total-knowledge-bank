<details>
<summary><h1>Coding Basics/White Belt/JavaScript + CLI</h1></summary>

💡 Tip: Click the arrows next to each heading to expand or collapse the content underneath.

<details>
<summary><h2>Key Concepts</h2></summary>

<details>
<summary><h3>Variables & Constants</h3></summary>

Q1: What is a variable?

A: A variable is a named box that stores information your program can use or change.

Q2: When should I use a variable?

A: Use a variable whenever a value might change while the program is running.

Q3: What is a constant?

A: A constant is a value that cannot be reassigned after it is created.

Q4: When should I use a constant instead of a variable?

A: Use a constant for values that should always stay the same, like PI or your app's name.

Q5: Why should I use meaningful variable names?

A: Good names make your code much easier to read and understand.

Q6: How do I create a variable?

A:

```jsx
let age = 25;
```

Q7: How do I create a constant?

A:

```jsx
const PI = 3.14159;
```

Q8: Can I change a variable later?

A: Yes.

```jsx
let score = 10;
score = 20;
```

Q9: Can I change a constant later?

A: No. Constants cannot be reassigned.

Q10: Why are variables one of the most important parts of programming?

A: They let your program remember information while it runs.

</details>

<details>
<summary><h3>Data Types</h3></summary>

Q11: What is a data type?

A: A data type tells JavaScript what kind of information is being stored.

Q12: What is a number?

A: A number stores whole numbers and decimal numbers.

```jsx
let apples = 10;
let price = 4.99;
```

Q13: What is a string?

A: A string stores text.

```jsx
let name = "Alice";
```

Q14: What is a boolean?

A: A boolean stores either true or false.

```jsx
let isRunning = true;
```

Q15: What is null?

A: Null means a variable intentionally has no value.

```jsx
let user = null;
```

Q16: What is undefined?

A: Undefined means a variable has not been given a value yet.

```jsx
let score;
```

Q17: When should I use a number instead of a string?

A: Use a number for math and a string for text.

Q18: Why should I pick the correct data type?

A: It helps prevent bugs and makes your code easier to understand.

Q19: Can one variable hold different data types?

A: Yes, JavaScript allows it, but it's usually better to keep one purpose per variable.

Q20: How do I know which data type to choose?

A: Ask yourself if you're storing a number, text, or true/false.

</details>

<details>
<summary><h3>Input / Output (CLI)</h3></summary>

Q21: What is output?

A: Output is information the program shows to the user.

Q22: How do I print text?

A:

```jsx
console.log("Hello!");
```

Q23: What is input?

A: Input is information the user gives to the program.

Q24: How do I read user input in Node.js?

A:

```jsx
const prompt = require("prompt-sync")();

const name = prompt("Enter your name: ");
```

Q25: Why does user input start as a string?

A: Everything typed on the keyboard starts as text.

Q26: How do I convert input into a number?

A:

```jsx
let age = Number(prompt("Age: "));
```

Q27: When should I use console.log()?

A: Use it whenever you want to display information in the terminal.

Q28: Why should I ask users for input?

A: It makes your program interactive.

Q29: How do I print variables?

A:

```jsx
console.log(name);
```

Q30: What happens if the user enters invalid data?

A: Your program may behave incorrectly unless you validate the input.

</details>

<details>
<summary><h3>Basic Math Operations</h3></summary>

Q31: What math operators does JavaScript have?

A: +, -, *, /, and %.

Q32: How do I add numbers?

A:

```jsx
let total = 5 + 3;
```

Q33: How do I subtract numbers?

A:

```jsx
let result = 10 - 4;
```

Q34: How do I multiply numbers?

A:

```jsx
let area = 5 * 6;
```

Q35: How do I divide numbers?

A:

```jsx
let answer = 20 / 4;
```

Q36: What does the % operator do?

A: It gives the remainder after division.

```jsx
7 % 2
```

Q37: When should I use the remainder operator?

A: Use it to check if a number is even, odd, or evenly divisible.

Q38: Why should I store math results in variables?

A: So you can reuse them later.

Q39: Can I do math with variables?

A: Yes.

```jsx
let total = apples + oranges;
```

Q40: Why is math important in programming?

A: Many programs calculate money, scores, measurements, and statistics.

</details>

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

Q41: What is an if statement?

A: An if statement lets the program make decisions.

Q42: When should I use an if statement?

A: Whenever something should only happen if a condition is true.

Q43: What is an else statement?

A: Else runs when the if condition is false.

Q44: How do I write an if statement?

A:

```jsx
if (age >= 18) {
    console.log("Adult");
}
```

Q45: How do I use if and else together?

A:

```jsx
if (score >= 60) {
    console.log("Pass");
} else {
    console.log("Fail");
}
```

Q46: What is a condition?

A: A condition is a question with a true or false answer.

Q47: What comparison operators are commonly used?

A:

```
==
===
!=
<
>
<=
>=
```

Q48: Why are conditionals important?

A: They let your program react differently in different situations.

Q49: Can I check more than one condition?

A: Yes.

```jsx
if (age >= 18 && hasID) {
    console.log("Access granted");
}
```

Q50: What is the easiest way to think about an if statement?

A: Think of it as asking a yes-or-no question before doing something.

</details>

<details>
<summary><h3>Random Numbers</h3></summary>

Q51: What is a random number?

A: A number chosen unpredictably from a range.

Q52: When should I use random numbers?

A: For games, simulations, or random choices.

Q53: How do I generate a random decimal?

A:

```jsx
let value = Math.random();
```

Q54: How do I generate a random whole number from 1 to 10?

A:

```jsx
let number = Math.floor(Math.random() * 10) + 1;
```

Q55: What does Math.random() return?

A: A decimal from 0 (inclusive) up to 1 (exclusive).

Q56: Why do I use Math.floor()?

A: It removes the decimal portion to create a whole number.

Q57: Can I generate random decimal numbers?

A: Yes.

```jsx
let value = Math.random();
```

Q58: How can I simulate rolling a die?

A:

```jsx
let roll = Math.floor(Math.random() * 6) + 1;
```

Q59: How can I randomly choose between true and false?

A:

```jsx
let result = Math.random() < 0.5;
```

Q60: Why are random numbers useful?

A: They make programs less predictable and more interesting by creating different results each time.

</details>

</details>

<details>
<summary><h2>Code Syntax</h2></summary>

<details>
<summary><h3>Variables & Constants</h3></summary>

Q1: I want to store a player's name in my program.

A:

```jsx
let playerName = "John";
```

Q2: I want to store a score that will change during the game.

A:

```jsx
let score = 0;
```

Q3: I want to store the value of PI that should never change.

A:

```jsx
const PI = 3.14159;
```

Q4: I want to store whether a player is alive or dead.

A:

```jsx
let isAlive = true;
```

Q5: I want to store a fixed game title.

A:

```jsx
const gameTitle = "Space Battle";
```

Q6: I want to increase a score by 10.

A:

```jsx
score += 10;
```

Q7: I want to reset a score to zero.

A:

```jsx
score = 0;
```

Q8: I want to store a player's age.

A:

```jsx
let age = 25;
```

Q9: I want to store a decimal health value.

A:

```jsx
let health = 75.5;
```

Q10: I want to update a player's name.

A:

```jsx
playerName = "Alex";
```

</details>

<details>
<summary><h3>Data Types</h3></summary>

Q11: I want to store whole numbers only.

A:

```jsx
let level = 1;
```

Q12: I want to store text entered by the user.

A:

```jsx
let input = prompt("Enter text:");
```

Q13: I want to store a yes/no value.

A:

```jsx
let hasKey = false;
```

Q14: I want to store a decimal number.

A:

```jsx
let price = 19.99;
```

Q15: I want to convert text into a number.

A:

```jsx
let age = Number(prompt("Enter age:"));
```

Q16: I want to store a very large number.

A:

```jsx
let distance = 1000000000;
```

Q17: I want to store multiple words.

A:

```jsx
let message = "Hello World";
```

Q18: I want to store whether a door is open.

A:

```jsx
let isOpen = true;
```

Q19: I want to store a player's username.

A:

```jsx
let username = "Player1";
```

Q20: I want to convert a string into a decimal number.

A:

```jsx
let price = parseFloat(prompt("Enter price:"));
```

</details>

<details>
<summary><h3>Input / Output (CLI)</h3></summary>

Q21: I want to print a message to the terminal.

A:

```jsx
console.log("Hello Player");
```

Q22: I want to ask the user for their name.

A:

```jsx
let name = prompt("Enter your name:");
```

Q23: I want to display the user's name.

A:

```jsx
console.log(name);
```

Q24: I want to ask for a number.

A:

```jsx
let number = Number(prompt("Enter a number:"));
```

Q25: I want to display a score.

A:

```jsx
console.log("Score:", score);
```

Q26: I want to display text and a variable together.

A:

```jsx
console.log("Hello", name);
```

Q27: I want to print a blank line.

A:

```jsx
console.log();
```

Q28: I want to display a welcome message.

A:

```jsx
console.log("Welcome to the game!");
```

Q29: I want to show the value of two variables.

A:

```jsx
console.log(name, score);
```

Q30: I want to ask for two numbers.

A:

```jsx
let num1 = Number(prompt("First number:"));
let num2 = Number(prompt("Second number:"));
```

</details>

<details>
<summary><h3>Basic Math Operations</h3></summary>

Q31: I want to add two numbers.

A:

```jsx
let result = a + b;
```

Q32: I want to subtract two numbers.

A:

```jsx
let result = a - b;
```

Q33: I want to multiply two numbers.

A:

```jsx
let result = a * b;
```

Q34: I want to divide two numbers.

A:

```jsx
let result = a / b;
```

Q35: I want to find the remainder after division.

A:

```jsx
let remainder = a % b;
```

Q36: I want to increase a variable by 1.

A:

```jsx
count++;
```

Q37: I want to decrease a variable by 1.

A:

```jsx
count--;
```

Q38: I want to add 5 to a score.

A:

```jsx
score += 5;
```

Q39: I want to double a value.

A:

```jsx
value *= 2;
```

Q40: I want to average two numbers.

A:

```jsx
let average = (a + b) / 2;
```

</details>

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

Q41: I want to check if a player is old enough.

A:

```jsx
if (age >= 18) {
    console.log("Allowed");
}
```

Q42: I want to block underage users.

A:

```jsx
if (age < 18) {
    console.log("Blocked");
}
```

Q43: I want to handle both pass and fail.

A:

```jsx
if (score >= 50) {
    console.log("Pass");
} else {
    console.log("Fail");
}
```

Q44: I want to check if a number equals 10.

A:

```jsx
if (number === 10) {
    console.log("Match");
}
```

Q45: I want to check if two conditions are true.

A:

```jsx
if (hasKey && doorLocked) {
    console.log("Open door");
}
```

Q46: I want to check if either condition is true.

A:

```jsx
if (isAdmin || isModerator) {
    console.log("Access granted");
}
```

Q47: I want to check if a number is not zero.

A:

```jsx
if (number !== 0) {
    console.log("Valid");
}
```

Q48: I want to handle multiple conditions.

A:

```jsx
if (score > 80) {
    console.log("A");
} else if (score > 50) {
    console.log("B");
} else {
    console.log("C");
}
```

Q49: I want to check if a user is logged in.

A:

```jsx
if (isLoggedIn) {
    console.log("Welcome");
}
```

Q50: I want to stop empty input.

A:

```jsx
if (input === "") {
    console.log("Invalid input");
}
```

</details>

<details>
<summary><h3>Random Numbers</h3></summary>

Q51: I want to generate a random number between 1 and 10.

A:

```jsx
let number = Math.floor(Math.random() * 10) + 1;
```

Q52: I want to simulate rolling a die.

A:

```jsx
let roll = Math.floor(Math.random() * 6) + 1;
```

Q53: I want to randomly pick true or false.

A:

```jsx
let result = Math.random() < 0.5;
```

Q54: I want to generate a random decimal.

A:

```jsx
let value = Math.random();
```

Q55: I want to generate a random number between 50 and 100.

A:

```jsx
let value = Math.floor(Math.random() * 51) + 50;
```

Q56: I want to simulate a coin flip.

A:

```jsx
let flip = Math.random() < 0.5 ? "Heads" : "Tails";
```

Q57: I want to randomly increase score by 1 or 2.

A:

```jsx
score += Math.floor(Math.random() * 2) + 1;
```

Q58: I want to randomly choose a name.

A:

```jsx
let names = ["Alex", "Sam", "Jordan"];
let pick = names[Math.floor(Math.random() * names.length)];
```

Q59: I want to generate a random damage value.

A:

```jsx
let damage = Math.floor(Math.random() * 11) + 5;
```

Q60: I want to randomly decide if an attack hits.

A:

```jsx
let hit = Math.random() < 0.75;
```

</details>

</details>

<details>
<summary><h2>Flowcharts + Key</h2></summary>

<details>
<summary><h3>Flowchart shape key</h3></summary>

| Text notation | Actual flowchart shape | Purpose |
| --- | --- | --- |
| `([ START / END ])` | **Oval / Terminator** | Start or end |
| `[ Process ]` | **Rectangle** | Calculation, assignment, setup |
| `[/ Input / Output /]` | **Parallelogram** | User input or console output |
| `{ Condition? }` | **Diamond** | Decision / branching |
| `↓` | **Arrow** | Direction of execution |

---

</details>

<details>
<summary><h3>Project 1: Simple Calculator</h3></summary>

<details>
<summary><h4>Text-based flowchart</h4></summary>

```
             ([ START ])
                  |
                  ↓
      [ Import prompt-sync ]
                  |
                  ↓
       [/ Ask for first number /]
                  |
                  ↓
       [/ Read user input /]
                  |
                  ↓
       [ Convert input to Number ]
                  |
                  ↓
       [/ Ask for second number /]
                  |
                  ↓
       [/ Read user input /]
                  |
                  ↓
       [ Convert input to Number ]
                  |
                  ↓
       [ Calculate addition
         add = num1 + num2 ]
                  |
                  ↓
       [ Calculate subtraction
         subtract = num1 - num2 ]
                  |
                  ↓
       [ Calculate multiplication
         multiply = num1 * num2 ]
                  |
                  ↓
       [ Calculate division
         divide = num1 / num2 ]
                  |
                  ↓
       [/ Display addition /]
                  |
                  ↓
       [/ Display subtraction /]
                  |
                  ↓
       [/ Display multiplication /]
                  |
                  ↓
       [/ Display division /]
                  |
                  ↓
              ([ END ])
```

</details>

<details>
<summary><h4>Shape breakdown</h4></summary>

- Import library → **Process**
- Ask user → **Input/Output**
- Read input → **Input/Output**
- `Number()` conversion → **Process**
- Math calculations → **Process**
- `console.log()` → **Input/Output**
- End → **Terminator**

</details>

<details>
<summary><h4>Core structure</h4></summary>

```
Input
  ↓
Convert
  ↓
Calculate
  ↓
Output
```

---

</details>

</details>

<details>
<summary><h3>Project 2: Number Guessing Game</h3></summary>

<details>
<summary><h4>Text-based flowchart</h4></summary>

```
             ([ START ])
                  |
                  ↓
       [ Import prompt-sync ]
                  |
                  ↓
       [ Generate random number
             between 1–10 ]
                  |
                  ↓
       [/ Ask user for guess /]
                  |
                  ↓
       [/ Read user input /]
                  |
                  ↓
       [ Convert guess to Number ]
                  |
                  ↓
        { guess === secret? }
             /           \
           YES            NO
            |              |
            ↓              ↓
    [/ Display          [/ Display
       "Correct!" /]       "Wrong!"
                            + secret /]
            |              |
            └───────┬──────┘
                    ↓
                ([ END ])
```

</details>

<details>
<summary><h4>Shape breakdown</h4></summary>

- Import `prompt-sync` → **Process**
- Generate random number → **Process**
- Ask for guess → **Input/Output**
- Read guess → **Input/Output**
- Convert guess → **Process**
- Compare guess → **Decision**
- Display result → **Input/Output**
- End → **Terminator**

</details>

<details>
<summary><h4>Core structure</h4></summary>

```
Generate random number
        ↓
    Get input
        ↓
    Compare
     /     \
 Correct   Wrong
```

This is your basic JavaScript:

```
if
else
```

pattern.

---

</details>

</details>

<details>
<summary><h3>Project 3: Login Checker</h3></summary>

<details>
<summary><h4>Text-based flowchart</h4></summary>

```
             ([ START ])
                  |
                  ↓
       [ Import prompt-sync ]
                  |
                  ↓
       [ Store correct
         username/password ]
                  |
                  ↓
       [/ Ask for username /]
                  |
                  ↓
       [/ Read username /]
                  |
                  ↓
       [/ Ask for password /]
                  |
                  ↓
       [/ Read password /]
                  |
                  ↓
       { Username correct
         AND
         Password correct? }
             /          \
           YES           NO
            |             |
            ↓             ↓
 [/ Display "Access     [/ Display "Access
      Granted" /]             Denied" /]
            |             |
            └──────┬──────┘
                   ↓
               ([ END ])
```

</details>

<details>
<summary><h4>Shape breakdown</h4></summary>

- Import library → **Process**
- Store credentials → **Process**
- Ask/read username → **Input/Output**
- Ask/read password → **Input/Output**
- Compare credentials → **Decision**
- Display access result → **Input/Output**
- End → **Terminator**

</details>

<details>
<summary><h4>Core logic</h4></summary>

```
Username matches?
       +
Password matches?
       ↓
      &&
       ↓
   Both true?
    /     \
  YES      NO
   ↓        ↓
Granted   Denied
```

The important programming concept here is the JavaScript **logical AND operator**:

```
username===correctUsername&&password===correctPassword
```

---

</details>

</details>

<details>
<summary><h3>Project 4: Grade Calculator</h3></summary>

This one demonstrates an **`if → else if → else` decision chain**.

<details>
<summary><h4>Text-based flowchart</h4></summary>

```
             ([ START ])
                  |
                  ↓
       [ Import prompt-sync ]
                  |
                  ↓
       [/ Ask for score /]
                  |
                  ↓
       [/ Read user input /]
                  |
                  ↓
       [ Convert input to Number ]
                  |
                  ↓
           { score >= 90? }
             /          \
           YES           NO
            |             |
            ↓             ↓
     [/ Display A /]   { score >= 80? }
                           /        \
                         YES         NO
                          |           |
                          ↓           ↓
                   [/ Display B /] { score >= 70? }
                                      /       \
                                    YES        NO
                                     |          |
                                     ↓          ↓
                              [/ Display C /] { score >= 60? }
                                                 /      \
                                               YES       NO
                                                |         |
                                                ↓         ↓
                                         [/ Display D /] [/ Display F /]
                                                |         |
                                                └────┬────┘
                                                     ↓
                                                 ([ END ])
```

</details>

<details>
<summary><h4>Shape breakdown</h4></summary>

- Import library → **Process**
- Ask for score → **Input/Output**
- Read score → **Input/Output**
- Convert to Number → **Process**
- Each `score >= X` → **Decision**
- Display grade → **Input/Output**
- End → **Terminator**

</details>

<details>
<summary><h4>Core logic</h4></summary>

```
score >= 90?
   │
   ├── YES → A
   │
   └── NO
        ↓
     score >= 80?
        │
        ├── YES → B
        │
        └── NO
             ↓
          score >= 70?
             │
             ├── YES → C
             │
             └── NO
                  ↓
               score >= 60?
                  │
                  ├── YES → D
                  │
                  └── NO → F
```

This is a good visual representation of **multiple mutually exclusive conditions**.

---

</details>

</details>

<details>
<summary><h3>Project 5: Dice Battle</h3></summary>

<details>
<summary><h4>Text-based flowchart</h4></summary>

```
             ([ START ])
                  |
                  ↓
       [ Generate Player 1
         random roll 1–6 ]
                  |
                  ↓
       [ Generate Player 2
         random roll 1–6 ]
                  |
                  ↓
       [/ Display Player 1 roll /]
                  |
                  ↓
       [/ Display Player 2 roll /]
                  |
                  ↓
        { player1 > player2? }
             /           \
           YES            NO
            |              |
            ↓              ↓
 [/ Display "Player 1   { player2 > player1? }
       Wins!" /]             /          \
                            YES           NO
                             |             |
                             ↓             ↓
                    [/ Display "Player 2  [/ Display
                         Wins!" /]          "It's a Tie!" /]
                             |             |
                             └──────┬──────┘
                                    |
                    ┌───────────────┘
                    ↓
                ([ END ])
```

</details>

<details>
<summary><h4>Shape breakdown</h4></summary>

- Generate Player 1 roll → **Process**
- Generate Player 2 roll → **Process**
- Display rolls → **Input/Output**
- Compare Player 1 > Player 2 → **Decision**
- Compare Player 2 > Player 1 → **Decision**
- Display winner/tie → **Input/Output**
- End → **Terminator**

</details>

<details>
<summary><h4>Core logic</h4></summary>

```
        Player 1 > Player 2?
             /          \
           YES           NO
            ↓             ↓
       Player 1 wins   Player 2 > Player 1?
                           /          \
                         YES           NO
                          ↓             ↓
                    Player 2 wins      Tie
```

This demonstrates an **`if → else if → else` decision tree**.

---

</details>

</details>

<details>
<summary><h3>All 5 Projects — Complexity Progression</h3></summary>

These five actually form a nice progression for your JavaScript project breakdown system:

```
PROJECT 1
Simple Calculator
        ↓
Sequential Logic
        ↓
Input → Process → Output
        ↓
PROJECT 2
Number Guessing
        ↓
Basic Decision
        ↓
Input → Process → Decision → Output
        ↓
PROJECT 3
Login Checker
        ↓
Boolean Logic
        ↓
Input → AND Condition → Output
        ↓
PROJECT 4
Grade Calculator
        ↓
Decision Chain
        ↓
if → else if → else
        ↓
PROJECT 5
Dice Battle
        ↓
Multiple Decisions
        ↓
Random Data → Decision Tree → Output
```

<details>
<summary><h4>The universal pattern</h4></summary>

You can also boil nearly every one of these beginner projects down to:

```
             ([ START ])
                  |
                  ↓
             INPUT
        [/ Input /]
                  |
                  ↓
            PROCESS
          [ Process ]
                  |
                  ↓
           DECISION?
          { Condition? }
             /     \
           YES      NO
            |        |
            ↓        ↓
         OUTPUT    OUTPUT
     [/ Output /] [/ Output /]
            \        /
             \      /
              ↓    ↓
             ([ END ])
```

</details>

</details>

</details>

<details>
<summary><h2>Sample Projects</h2></summary>

<details>
<summary><h3>Project 1: Simple Calculator</h3></summary>

<details>
<summary><h4>What it does</h4></summary>

Asks the user for two numbers, then displays the results of basic math operations.

</details>

<details>
<summary><h4>Step-by-step</h4></summary>

1. Import the prompt-sync library.
2. Ask the user for the first number.
3. Ask the user for the second number.
4. Perform addition, subtraction, multiplication, and division.
5. Display each result.

```jsx
// Step 1: Import prompt-sync so we can read user input
const prompt = require("prompt-sync")();

// Step 2: Ask the user for the first number
let num1 = Number(prompt("Enter the first number: "));

// Step 3: Ask the user for the second number
let num2 = Number(prompt("Enter the second number: "));

// Step 4: Perform the calculations
let add = num1 + num2;
let subtract = num1 - num2;
let multiply = num1 * num2;
let divide = num1 / num2;

// Step 5: Display the results
console.log("Addition:", add);
console.log("Subtraction:", subtract);
console.log("Multiplication:", multiply);
console.log("Division:", divide);
```

---

</details>

</details>

<details>
<summary><h3>Project 2: Number Guessing Game</h3></summary>

<details>
<summary><h4>What it does</h4></summary>

The computer picks a random number from 1–10. The user tries to guess it.

</details>

<details>
<summary><h4>Step-by-step</h4></summary>

1. Import the prompt-sync library.
2. Generate a random number.
3. Ask the user for a guess.
4. Compare the guess to the random number.
5. Display whether the guess was correct.

```jsx
// Step 1: Import prompt-sync
const prompt = require("prompt-sync")();

// Step 2: Generate a random number between 1 and 10
let secret = Math.floor(Math.random() * 10) + 1;

// Step 3: Ask the user for a guess
let guess = Number(prompt("Guess a number (1-10): "));

// Step 4: Compare the guess to the secret number
if (guess === secret)
{
    // Step 5A: User guessed correctly
    console.log("Correct!");
}
else
{
    // Step 5B: User guessed incorrectly
    console.log("Wrong! The number was", secret);
}
```

---

</details>

</details>

<details>
<summary><h3>Project 3: Login Checker</h3></summary>

<details>
<summary><h4>What it does</h4></summary>

Checks whether the username and password match the stored values.

</details>

<details>
<summary><h4>Step-by-step</h4></summary>

1. Import the prompt-sync library.
2. Store the correct username and password.
3. Ask the user for their username.
4. Ask the user for their password.
5. Compare both values.
6. Display whether login succeeded.

```jsx
// Step 1: Import prompt-sync
const prompt = require("prompt-sync")();

// Step 2: Store the correct login information
const correctUsername = "admin";
const correctPassword = "1234";

// Step 3: Ask for the username
let username = prompt("Username: ");

// Step 4: Ask for the password
let password = prompt("Password: ");

// Step 5: Compare both values
if (username === correctUsername && password === correctPassword)
{
    // Step 6A: Login successful
    console.log("Access Granted");
}
else
{
    // Step 6B: Login failed
    console.log("Access Denied");
}
```

---

</details>

</details>

<details>
<summary><h3>Project 4: Grade Calculator</h3></summary>

<details>
<summary><h4>What it does</h4></summary>

Converts a numeric score into a letter grade.

</details>

<details>
<summary><h4>Step-by-step</h4></summary>

1. Import the prompt-sync library.
2. Ask the user for a score.
3. Convert the input into a number.
4. Determine the correct letter grade.
5. Display the grade.

```jsx
// Step 1: Import prompt-sync
const prompt = require("prompt-sync")();

// Step 2: Ask for the student's score
let score = Number(prompt("Enter score (0-100): "));

// Step 3 & 4: Determine the letter grade
if (score >= 90)
{
    console.log("Grade: A");
}
else if (score >= 80)
{
    console.log("Grade: B");
}
else if (score >= 70)
{
    console.log("Grade: C");
}
else if (score >= 60)
{
    console.log("Grade: D");
}
else
{
    console.log("Grade: F");
}
```

---

</details>

</details>

<details>
<summary><h3>Project 5: Dice Battle</h3></summary>

<details>
<summary><h4>What it does</h4></summary>

Two players roll a six-sided die. The higher roll wins.

</details>

<details>
<summary><h4>Step-by-step</h4></summary>

1. Generate Player 1's roll.
2. Generate Player 2's roll.
3. Display both rolls.
4. Compare the rolls.
5. Announce the winner.

```jsx
// Step 1: Generate Player 1's dice roll
let player1 = Math.floor(Math.random() * 6) + 1;

// Step 2: Generate Player 2's dice roll
let player2 = Math.floor(Math.random() * 6) + 1;

// Step 3: Display both rolls
console.log("Player 1 rolled:", player1);
console.log("Player 2 rolled:", player2);

// Step 4: Compare the rolls
if (player1 > player2)
{
    // Step 5A: Player 1 wins
    console.log("Player 1 Wins!");
}
else if (player2 > player1)
{
    // Step 5B: Player 2 wins
    console.log("Player 2 Wins!");
}
else
{
    // Step 5C: Tie game
    console.log("It's a Tie!");
}
```

</details>

</details>

</details>

</details>