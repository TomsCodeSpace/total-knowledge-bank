
<details>
<summary><h1>Coding Basics/White Belt/Java + CLI</h1></summary>

💡 Tip: Click the arrows next to each heading to expand or collapse the content underneath.

<details>
<summary><h2>Key Concepts</h2></summary>

<details>
<summary><h3>Variables & Constants</h3></summary>

Q1: What is a variable in Java?

A: A variable is a named container that stores data your program can use or change.

Q2: When should I use a variable?

A: Use it when a value will change while the program runs.

Q3: How do I create a variable?

A:

```java
int score = 10;
```

Q4: What is a constant in Java?

A: A constant is a value that cannot change after it is set.

Q5: How do I create a constant?

A:

```java
final int MAX_SCORE = 100;
```

Q6: When should I use a constant?

A: When the value should never change, like limits or settings.

Q7: Why use variables instead of hardcoding values?

A: So your program is flexible and easier to update.

Q8: Can variables change in Java?

A: Yes, unless marked `final`.

Q9: What does `final` mean?

A: It locks a value so it cannot change.

Q10: Why are variables important?

A: They let programs remember information.

</details>

<details>
<summary><h3>Data Types</h3></summary>

Q11: What is a data type?

A: It tells Java what kind of data is stored.

Q12: What is an `int`?

A:

```java
int age = 20;
```

Q13: What is a `double`?

A:

```java
double price = 4.99;
```

Q14: What is a `String`?

A:

```java
String name = "Alex";
```

Q15: What is a `boolean`?

A:

```java
boolean isAlive = true;
```

Q16: When should I use `int` vs `double`?

A: `int` for whole numbers, `double` for decimals.

Q17: Why do data types matter?

A: They prevent wrong operations.

Q18: Can Java change types automatically?

A: Sometimes, but it can cause errors.

Q19: What is `char`?

A:

```java
char grade = 'A';
```

Q20: Why use correct data types?

A: To keep code predictable and safe.

</details>

<details>
<summary><h3>Input / Output (CLI)</h3></summary>

Q21: How do I print text in Java?

A:

```java
System.out.println("Hello");
```

Q22: What is output?

A: Information shown to the user.

Q23: What is input in Java CLI?

A: Data the user types in the terminal.

Q24: How do I read input?

A:

```java
import java.util.Scanner;

Scanner sc = new Scanner(System.in);
String name = sc.nextLine();
```

Q25: Why use `Scanner`?

A: It lets Java read user input.

Q26: How do I read numbers?

A:

```java
int num = sc.nextInt();
```

Q27: Why convert input?

A: Because input is text by default.

Q28: What happens if input is wrong type?

A: The program crashes.

Q29: How do I print variables?

A:

```java
System.out.println(name);
```

Q30: Why use CLI input?

A: To make programs interactive.

</details>

<details>
<summary><h3>Basic Math Operations</h3></summary>

Q31: How do I add numbers in Java?

A:

```java
int sum = a + b;
```

Q32: How do I subtract?

A:

```java
int result = a - b;
```

Q33: How do I multiply?

A:

```java
int result = a * b;
```

Q34: How do I divide?

A:

```java
int result = a / b;
```

Q35: What is modulus?

A:

```java
int r = a % b;
```

Q36: When should I use modulus?

A: To find remainders or even/odd checks.

Q37: Why store math results?

A: So they can be reused later.

Q38: What happens when dividing integers?

A: Decimal part is removed.

Q39: How to get accurate division?

A:

```java
double result = (double)a / b;
```

Q40: Why is math important?

A: Many programs calculate data.

</details>

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

Q41: What is an `if` statement?

A: A decision maker in code.

Q42: When should I use `if`?

A: When something depends on a condition.

Q43: How do I write `if`?

A:

```java
if (age >= 18) {
    System.out.println("Adult");
}
```

Q44: What is `else`?

A: What happens when `if` is false.

Q45: How do I use `else`?

A:

```java
if (score >= 50) {
    System.out.println("Pass");
} else {
    System.out.println("Fail");
}
```

Q46: What is a condition?

A: A true/false question.

Q47: What are comparison operators?

A:

```
== != < > <= >=
```

Q48: Why use conditions?

A: To make decisions in programs.

Q49: Can I use multiple conditions?

A:

```java
if (age > 18 && hasID)
```

Q50: What does `&&` mean?

A: Both conditions must be true.

</details>

<details>
<summary><h3>Random Numbers</h3></summary>

Q51: How do I generate random numbers in Java?

A:

```java
import java.util.Random;

Random rand = new Random();
int num = rand.nextInt(10);
```

Q52: What does `nextInt(10)` mean?

A: Random number from 0–9.

Q53: How do I get 1–10 instead of 0–9?

A:

```java
int num = rand.nextInt(10) + 1;
```

Q54: When should I use random numbers?

A: Games, simulations, randomness.

Q55: Why use the `Random` class?

A: It generates unpredictable values.

Q56: How do I simulate a dice roll?

A:

```java
int roll = rand.nextInt(6) + 1;
```

Q57: How do I pick true/false randomly?

A:

```java
boolean b = rand.nextBoolean();
```

Q58: Why not use `Math.random()` for everything?

A: The `Random` class is more flexible.

Q59: How do I randomize decisions?

A:

```java
if (rand.nextInt(100) < 50)
```

Q60: Why is randomness useful?

A: It makes programs less predictable and more interactive.

</details>
</details>

<details>
<summary><h2>Code Syntax</h2></summary>

<details>
<summary><h3>Variables & Constants</h3></summary>

Q1: I want to store a player's name.

A:

```java
String playerName = "Alex";
```

Q2: I want to store a score that changes during the game.

A:

```java
int score = 0;
```

Q3: I want to store a fixed max value that never changes.

A:

```java
final int MAX = 100;
```

Q4: I want to update a player's score.

A:

```java
score += 10;
```

Q5: I want to reset a score.

A:

```java
score = 0;
```

Q6: I want to store a player's health.

A:

```java
int health = 100;
```

Q7: I want to store whether a player is alive.

A:

```java
boolean isAlive = true;
```

Q8: I want to store a decimal price.

A:

```java
double price = 19.99;
```

Q9: I want to store a single character grade.

A:

```java
char grade = 'A';
```

Q10: I want to update a username.

A:

```java
playerName = "Jordan";
```

</details>

<details>
<summary><h3>Input / Output (CLI)</h3></summary>

Q11: I want to print a message to the console.

A:

```java
System.out.println("Hello World");
```

Q12: I want to ask the user for input.

A:

```java
Scanner sc = new Scanner(System.in);
String name = sc.nextLine();
```

Q13: I want to read a number from user input.

A:

```java
int age = sc.nextInt();
```

Q14: I want to display a variable.

A:

```java
System.out.println(score);
```

Q15: I want to combine text and variables in output.

A:

```java
System.out.println("Score: " + score);
```

Q16: I want to clear a line conceptually in CLI (simulate).

A:

```java
System.out.println("\n\n");
```

Q17: I want to pause for input.

A:

```java
sc.nextLine();
```

Q18: I want to show a welcome message.

A:

```java
System.out.println("Welcome!");
```

Q19: I want to ask for two inputs.

A:

```java
int a = sc.nextInt();
int b = sc.nextInt();
```

Q20: I want to display both inputs.

A:

```java
System.out.println(a + " " + b);
```

</details>

<details>
<summary><h3>Basic Math Operations</h3></summary>

Q21: I want to add two numbers.

A:

```java
int result = a + b;
```

Q22: I want to subtract two numbers.

A:

```java
int result = a - b;
```

Q23: I want to multiply two numbers.

A:

```java
int result = a * b;
```

Q24: I want to divide two numbers.

A:

```java
int result = a / b;
```

Q25: I want to get remainder.

A:

```java
int r = a % b;
```

Q26: I want to increase a value by 1.

A:

```java
score++;
```

Q27: I want to decrease a value by 1.

A:

```java
score--;
```

Q28: I want to double a number.

A:

```java
value *= 2;
```

Q29: I want to average two numbers.

A:

```java
double avg = (a + b) / 2.0;
```

Q30: I want to calculate total cost.

A:

```java
double total = price * quantity;
```

</details>

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

Q31: I want to check if someone is an adult.

A:

```java
if (age >= 18) {
    System.out.println("Adult");
}
```

Q32: I want to block underage users.

A:

```java
if (age < 18) {
    System.out.println("Blocked");
}
```

Q33: I want to check pass/fail.

A:

```java
if (score >= 50) {
    System.out.println("Pass");
} else {
    System.out.println("Fail");
}
```

Q34: I want to check equality.

A:

```java
if (a == b) {
    System.out.println("Equal");
}
```

Q35: I want to check not equal.

A:

```java
if (a != b) {
    System.out.println("Not equal");
}
```

Q36: I want to check greater than.

A:

```java
if (score > 80) {
    System.out.println("High score");
}
```

Q37: I want to check multiple conditions.

A:

```java
if (age > 18 && hasID) {
    System.out.println("Allowed");
}
```

Q38: I want to check either condition.

A:

```java
if (isAdmin || isMod) {
    System.out.println("Access");
}
```

Q39: I want to assign grade A/B/C.

A:

```java
if (score >= 90) {
    System.out.println("A");
} else if (score >= 80) {
    System.out.println("B");
} else {
    System.out.println("C");
}
```

Q40: I want to handle invalid input.

A:

```java
if (input.isEmpty()) {
    System.out.println("Invalid");
}
```

</details>

<details>
<summary><h3>Random Numbers</h3></summary>

Q41: I want to generate a random number 1–10.

A:

```java
Random rand = new Random();
int num = rand.nextInt(10) + 1;
```

Q42: I want to simulate a dice roll.

A:

```java
int roll = rand.nextInt(6) + 1;
```

Q43: I want a random true/false.

A:

```java
boolean b = rand.nextBoolean();
```

Q44: I want to randomly increase score.

A:

```java
score += rand.nextInt(5);
```

Q45: I want to randomly pick between two outcomes.

A:

```java
if (rand.nextInt(2) == 0) {
    System.out.println("Heads");
} else {
    System.out.println("Tails");
}
```

Q46: I want to generate random damage.

A:

```java
int damage = rand.nextInt(10) + 5;
```

Q47: I want to simulate chance (50%).

A:

```java
if (rand.nextInt(100) < 50)
```

Q48: I want to pick a random number range 50–100.

A:

```java
int num = rand.nextInt(51) + 50;
```

Q49: I want to randomly choose a name.

A:

```java
String[] names = {"Alex", "Sam", "Jordan"};
String pick = names[rand.nextInt(names.length)];
```

Q50: I want to simulate a critical hit chance.

A:

```java
boolean crit = rand.nextInt(100) < 25;
```

</details>

<details>
<summary><h3>Mixed CLI Logic</h3></summary>

Q51: I want to ask for a name and greet the user.

A:

```java
System.out.println("Hello " + sc.nextLine());
```

Q52: I want to add two user inputs.

A:

```java
int sum = sc.nextInt() + sc.nextInt();
```

Q53: I want to check if input is positive.

A:

```java
if (num > 0) {
    System.out.println("Positive");
}
```

Q54: I want to prevent division by zero.

A:

```java
if (b != 0) {
    System.out.println(a / b);
}
```

Q55: I want to repeat an action conditionally.

A:

```java
if (score > 100) {
    score = 100;
}
```

Q56: I want to display both name and score.

A:

```java
System.out.println(name + ": " + score);
```

Q57: I want to check login success.

A:

```java
if (user.equals("admin") && pass.equals("1234"))
```

Q58: I want to fail empty input.

A:

```java
if (input == null || input.isEmpty())
```

Q59: I want to compare two numbers safely.

A:

```java
System.out.println(Math.max(a, b));
```

Q60: I want to generate a random event trigger.

A:

```java
if (rand.nextInt(100) < 10) {
    System.out.println("Event triggered!");
}
```

</details>
</details>

<details>
<summary><h2>Flowcharts + Key</h2></summary>

<details>
<summary><h3>Flowchart Shape Key</h3></summary>

| Text notation | Actual flowchart shape | Meaning |
| --- | --- | --- |
| `([ START / END ])` | **Oval / Terminator** | Program beginning or ending |
| `[ Process ]` | **Rectangle** | Calculation, assignment, object creation, etc. |
| `[/ Input / Output /]` | **Parallelogram** | User input or printed output |
| `{ Condition? }` | **Diamond** | Decision / branching |
| `↓` | **Arrow** | Direction of program flow |

</details>

<details>
<summary><h3>Project 1: Simple CLI Calculator</h3></summary>

One extra detail here: the Java code contains a **ternary operator** to prevent division by zero:

```java
(b != 0) ? (a / b) : 0
```

So I'll represent that as a decision in the flowchart.

**Text-based flowchart**

```
             ([ START ])
                  |
                  ↓
       [ Create Scanner object ]
                  |
                  ↓
       [/ Ask for first number /]
                  |
                  ↓
       [/ Read integer a /]
                  |
                  ↓
       [/ Ask for second number /]
                  |
                  ↓
       [/ Read integer b /]
                  |
                  ↓
       [ Calculate addition
             add = a + b ]
                  |
                  ↓
       [ Calculate subtraction
             sub = a - b ]
                  |
                  ↓
       [ Calculate multiplication
             mul = a * b ]
                  |
                  ↓
             { b != 0? }
              /       \
            YES        NO
             |          |
             ↓          ↓
       [ div = a / b ] [ div = 0 ]
             |          |
             └────┬─────┘
                  ↓
       [/ Print addition result /]
                  |
                  ↓
       [/ Print subtraction result /]
                  |
                  ↓
       [/ Print multiplication result /]
                  |
                  ↓
       [/ Print division result /]
                  |
                  ↓
              ([ END ])
```

**Shape breakdown**

- Create `Scanner` → **Process**
- Ask for number → **Input/Output**
- Read number → **Input/Output**
- Addition/subtraction/multiplication → **Process**
- `b != 0` → **Decision**
- Calculate division → **Process**
- Print results → **Input/Output**
- End → **Terminator**

**Core concept**

```
Input
  ↓
Process
  ↓
Decision
  ↓
Process
  ↓
Output
```

</details>

<details>
<summary><h3>Project 2: Number Guessing Game</h3></summary>

**Text-based flowchart**

```
             ([ START ])
                  |
                  ↓
       [ Create Scanner object ]
                  |
                  ↓
       [ Create Random object ]
                  |
                  ↓
       [ Generate secret number
             between 1–10 ]
                  |
                  ↓
       [/ Ask user for guess /]
                  |
                  ↓
       [/ Read integer guess /]
                  |
                  ↓
          { guess == secret? }
             /            \
           YES             NO
            |               |
            ↓               ↓
[/ Print "Correct!" /] [/ Print "Wrong!"
                          + secret /]
            |               |
            └───────┬───────┘
                    ↓
                ([ END ])
```

**Shape breakdown**

- Create `Scanner` → **Process**
- Create `Random` → **Process**
- Generate secret → **Process**
- Ask/read guess → **Input/Output**
- Compare values → **Decision**
- Print result → **Input/Output**
- End → **Terminator**

**Core logic**

```
Generate Random
      ↓
Get Guess
      ↓
{ Guess == Secret? }
   /          \
 YES           NO
  ↓             ↓
Correct         Wrong
```

</details>

<details>
<summary><h3>Project 3: Login System</h3></summary>

**Text-based flowchart**

```
             ([ START ])
                  |
                  ↓
       [ Create Scanner object ]
                  |
                  ↓
       [ Store correct username
         and correct password ]
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
       { Username matches
         AND
         Password matches? }
             /          \
           YES           NO
            |             |
            ↓             ↓
[/ Print "Access       [/ Print "Access
      Granted" /]           Denied" /]
            |             |
            └──────┬──────┘
                   ↓
               ([ END ])
```

**Shape breakdown**

- Create `Scanner` → **Process**
- Store credentials → **Process**
- Ask for username → **Input/Output**
- Read username → **Input/Output**
- Ask for password → **Input/Output**
- Read password → **Input/Output**
- Compare credentials → **Decision**
- Print result → **Input/Output**
- End → **Terminator**

**Core logic**

The diamond represents:

```java
user.equals(correctUser) && pass.equals(correctPass)
```

Visually:

```
Username correct?
      +
Password correct?
      ↓
     AND
      ↓
 Both true?
  /      \
YES       NO
 ↓         ↓
Granted   Denied
```

</details>

<details>
<summary><h3>Project 4: Grade Calculator</h3></summary>

This is your **multi-condition decision tree**.

**Text-based flowchart**

```
             ([ START ])
                  |
                  ↓
       [ Create Scanner object ]
                  |
                  ↓
          [/ Ask for score /]
                  |
                  ↓
          [/ Read score /]
                  |
                  ↓
          { score >= 90? }
             /          \
           YES           NO
            |             |
            ↓             ↓
        [/ Print A /] { score >= 80? }
                          /        \
                        YES         NO
                         |           |
                         ↓           ↓
                   [/ Print B /] { score >= 70? }
                                    /       \
                                  YES        NO
                                   |          |
                                   ↓          ↓
                             [/ Print C /] { score >= 60? }
                                                /       \
                                              YES        NO
                                               |          |
                                               ↓          ↓
                                         [/ Print D /] [/ Print F /]
                                               |          |
                                               └────┬─────┘
                                                    ↓
                                                ([ END ])
```

**Shape breakdown**

- Create `Scanner` → **Process**
- Ask/read score → **Input/Output**
- `score >= 90` → **Decision**
- `score >= 80` → **Decision**
- `score >= 70` → **Decision**
- `score >= 60` → **Decision**
- Print grade → **Input/Output**
- End → **Terminator**

**Logic tree**

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

This is a good example of **sequentially narrowing down a set of possibilities**.

</details>

<details>
<summary><h3>Project 5: Dice Battle Simulator</h3></summary>

**Text-based flowchart**

```
             ([ START ])
                  |
                  ↓
       [ Create Random object ]
                  |
                  ↓
       [ Generate Player 1 roll
             between 1–6 ]
                  |
                  ↓
       [ Generate Player 2 roll
             between 1–6 ]
                  |
                  ↓
       [/ Print Player 1 roll /]
                  |
                  ↓
       [/ Print Player 2 roll /]
                  |
                  ↓
          { p1 > p2? }
             /       \
           YES        NO
            |          |
            ↓          ↓
[/ Print "Player 1   { p2 > p1? }
      Wins!" /]         /      \
                      YES       NO
                       |         |
                       ↓         ↓
               [/ Print "Player 2  [/ Print "Tie!" /]
                     Wins!" /]          |
                       |                 |
                       └────────┬────────┘
                                ↓
                            ([ END ])
```

**Shape breakdown**

- Create `Random` → **Process**
- Generate P1 roll → **Process**
- Generate P2 roll → **Process**
- Print rolls → **Input/Output**
- `p1 > p2` → **Decision**
- `p2 > p1` → **Decision**
- Print winner/tie → **Input/Output**
- End → **Terminator**

**Core logic**

```
         p1 > p2?
         /     \
       YES      NO
        ↓        ↓
    P1 Wins    p2 > p1?
               /      \
             YES       NO
              ↓         ↓
          P2 Wins      Tie
```

</details>

<details>
<summary><h3>All 5 Java Projects — Progression</h3></summary>

These line up nicely as a beginner Java progression:

```
PROJECT 1
Simple Calculator
       ↓
Sequential Processing
       ↓
Input → Process → Output
       ↓
PROJECT 2
Number Guessing
       ↓
Basic if/else
       ↓
Input → Random → Decision → Output
       ↓
PROJECT 3
Login System
       ↓
Boolean Logic
       ↓
Condition A AND Condition B
       ↓
PROJECT 4
Grade Calculator
       ↓
Multiple Conditions
       ↓
if → else if → else
       ↓
PROJECT 5
Dice Battle
       ↓
Multiple Branches
       ↓
if → else if → else
```

**Master flowchart for these Java projects**

```
                  ([ START ])
                       |
                       ↓
               [ SETUP PROGRAM ]
                       |
                       ↓
                 [/ GET INPUT /]
                       |
                       ↓
                  [ PROCESS ]
                       |
                       ↓
                 { DECISION? }
                   /       \
                 YES        NO
                  |          |
                  ↓          ↓
             [ PROCESS ] [ PROCESS ]
                  |          |
                  └────┬─────┘
                       ↓
                [/ OUTPUT /]
                       |
                       ↓
                   ([ END ])
```

</details>
</details>

<details>
<summary><h2>Sample Projects</h2></summary>

<details>
<summary><h3>Project 1: Simple CLI Calculator</h3></summary>

**What it does**

Takes two numbers from the user and performs math operations.

**Steps**

1. Create Scanner
2. Ask for first number
3. Ask for second number
4. Perform math
5. Print results

```java
import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        // Step 1: Ask for first number
        System.out.print("Enter first number: ");
        int a = sc.nextInt();

        // Step 2: Ask for second number
        System.out.print("Enter second number: ");
        int b = sc.nextInt();

        // Step 3: Perform calculations
        int add = a + b;
        int sub = a - b;
        int mul = a * b;
        int div = (b != 0) ? (a / b) : 0;

        // Step 4: Output results
        System.out.println("Add: " + add);
        System.out.println("Subtract: " + sub);
        System.out.println("Multiply: " + mul);
        System.out.println("Divide: " + div);
    }
}
```

</details>

<details>
<summary><h3>Project 2: Number Guessing Game</h3></summary>

**What it does**

User guesses a random number 1–10.

**Steps**

1. Generate random number
2. Ask user for guess
3. Compare values
4. Print result

```java
import java.util.Scanner;
import java.util.Random;

public class GuessGame {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        Random rand = new Random();

        // Step 1: Generate random number
        int secret = rand.nextInt(10) + 1;

        // Step 2: Ask user for guess
        System.out.print("Guess (1-10): ");
        int guess = sc.nextInt();

        // Step 3: Compare values
        if (guess == secret) {
            System.out.println("Correct!");
        } else {
            System.out.println("Wrong! It was " + secret);
        }
    }
}
```

</details>

<details>
<summary><h3>Project 3: Login System</h3></summary>

**What it does**

Checks username and password in CLI.

**Steps**

1. Store correct credentials
2. Ask for username
3. Ask for password
4. Compare
5. Show result

```java
import java.util.Scanner;

public class Login {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        // Step 1: Stored credentials
        String correctUser = "admin";
        String correctPass = "1234";

        // Step 2: Ask user input
        System.out.print("Username: ");
        String user = sc.nextLine();

        System.out.print("Password: ");
        String pass = sc.nextLine();

        // Step 3: Compare
        if (user.equals(correctUser) && pass.equals(correctPass)) {
            System.out.println("Access Granted");
        } else {
            System.out.println("Access Denied");
        }
    }
}
```

</details>

<details>
<summary><h3>Project 4: Grade Calculator</h3></summary>

**What it does**

Turns numeric score into letter grade.

**Steps**

1. Get score input
2. Check ranges
3. Print grade

```java
import java.util.Scanner;

public class GradeCalc {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        // Step 1: Get score
        System.out.print("Enter score: ");
        int score = sc.nextInt();

        // Step 2: Determine grade
        if (score >= 90) {
            System.out.println("A");
        } else if (score >= 80) {
            System.out.println("B");
        } else if (score >= 70) {
            System.out.println("C");
        } else if (score >= 60) {
            System.out.println("D");
        } else {
            System.out.println("F");
        }
    }
}
```

</details>

<details>
<summary><h3>Project 5: Dice Battle Simulator</h3></summary>

**What it does**

Two players roll dice; highest wins.

**Steps**

1. Create Random
2. Generate rolls
3. Compare values
4. Print winner

```java
import java.util.Random;

public class DiceBattle {
    public static void main(String[] args) {

        Random rand = new Random();

        // Step 1: Player 1 roll
        int p1 = rand.nextInt(6) + 1;

        // Step 2: Player 2 roll
        int p2 = rand.nextInt(6) + 1;

        // Step 3: Show rolls
        System.out.println("P1: " + p1);
        System.out.println("P2: " + p2);

        // Step 4: Determine winner
        if (p1 > p2) {
            System.out.println("Player 1 Wins!");
        } else if (p2 > p1) {
            System.out.println("Player 2 Wins!");
        } else {
            System.out.println("Tie!");
        }
    }
}
```

</details>
</details>

</details>
