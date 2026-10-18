<details>
<summary><h1>Coding Basics/White Belt/C# + CLI</h1></summary>

💡 Tip: Click the arrows next to each heading to expand or collapse the content underneath.

<details>
<summary><h2>Key Concepts</h2></summary>

<details>
<summary><h3>Variables and Constants</h3></summary>

**Q1: What is a variable?**

A: A variable is a named box that stores information your program can use or change.

**Q2: When should I use a variable?**

A: Use a variable whenever a value might change while the program is running.

**Q3: What is a constant?**

A: A constant is a value that cannot be changed after it is created.

**Q4: When should I use a constant instead of a variable?**

A: Use a constant for values that should always stay the same, like PI or the number of days in a week.

**Q5: Why should I use meaningful variable names?**

A: Good names make your code much easier to read and understand.

**Q6: How do I create a variable?**

A:

```csharp
int age = 25;
```

**Q7: How do I create a constant?**

A:

```csharp
const double Pi = 3.14159;
```

**Q8: Can I change a variable later?**

A: Yes.

```csharp
int score = 10;
score = 20;
```

**Q9: Can I change a constant later?**

A: No. Constants cannot be modified.

**Q10: Why are variables one of the most important parts of programming?**

A: They let your program remember information while it runs.

</details>

<details>
<summary><h3>Data Types</h3></summary>

**Q11: What is a data type?**

A: A data type tells C# what kind of information is being stored.

**Q12: What is an int?**

A: An int stores whole numbers.

```csharp
int apples = 10;
```

**Q13: What is a double?**

A: A double stores numbers with decimal places.

```csharp
double price = 4.99;
```

**Q14: What is a string?**

A: A string stores text.

```csharp
string name = "Alice";
```

**Q15: What is a char?**

A: A char stores a single character.

```csharp
char grade = 'A';
```

**Q16: What is a bool?**

A: A bool stores either true or false.

```csharp
bool isRunning = true;
```

**Q17: When should I use an int instead of a double?**

A: Use int for whole numbers and double for decimal numbers.

**Q18: Why should I pick the correct data type?**

A: It helps prevent bugs and makes your code more efficient.

**Q19: Can one variable hold different data types?**

A: No. A variable has one data type.

**Q20: How do I know which data type to choose?**

A: Ask yourself what kind of data you're storing: number, text, letter, or true/false.

</details>

<details>
<summary><h3>Input and Output</h3></summary>

**Q21: What is output?**

A: Output is information the program shows to the user.

**Q22: How do I display text?**

A:

```csharp
Console.WriteLine("Hello!");
```

**Q23: What is input?**

A: Input is information the user gives to the program.

**Q24: How do I read user input?**

A:

```csharp
string name = Console.ReadLine();
```

**Q25: Why does ReadLine() return a string?**

A: Everything typed on the keyboard starts as text.

**Q26: How do I convert text into a number?**

A:

```csharp
int age = int.Parse(Console.ReadLine());
```

**Q27: When should I use Console.Write()?**

A: Use it when you do not want the cursor to move to a new line.

**Q28: When should I use Console.WriteLine()?**

A: Use it when you want the next output to appear on a new line.

**Q29: Why should I ask users for input?**

A: It makes your program interactive instead of always doing the same thing.

**Q30: What happens if the user enters the wrong type of data?**

A: The program may crash unless you handle the error.

</details>

<details>
<summary><h3>Basic Math Operations</h3></summary>

**Q31: What math operators does C# have?**

A: +, -, *, /, and %.

**Q32: How do I add numbers?**

A:

```csharp
int total = 5 + 3;
```

**Q33: How do I subtract numbers?**

A:

```csharp
int result = 10 - 4;
```

**Q34: How do I multiply numbers?**

A:

```csharp
int area = 5 * 6;
```

**Q35: How do I divide numbers?**

A:

```csharp
int answer = 20 / 4;
```

**Q36: What does the % operator do?**

A: It gives the remainder after division.

```csharp
7 % 2
```

Result:

```
1
```

**Q37: When should I use the remainder operator?**

A: Use it to check if a number is even, odd, or evenly divisible.

**Q38: Why should I store math results in variables?**

A: So you can reuse the answer later.

**Q39: Can I do math with variables?**

A: Yes.

```csharp
int total = apples + oranges;
```

**Q40: Why is math important in programming?**

A: Many programs calculate values, measurements, scores, money, and statistics.

</details>

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

**Q41: What is an if statement?**

A: An if statement lets the program make decisions.

**Q42: When should I use an if statement?**

A: Use it whenever something should only happen if a condition is true.

**Q43: What is an else statement?**

A: Else runs when the if condition is false.

**Q44: How do I write an if statement?**

A:

```csharp
if (age >= 18)
{
    Console.WriteLine("Adult");
}
```

**Q45: How do I use if and else together?**

A:

```csharp
if (score >= 60)
{
    Console.WriteLine("Pass");
}
else
{
    Console.WriteLine("Fail");
}
```

**Q46: What is a condition?**

A: A condition is a question that is either true or false.

**Q47: What comparison operators are commonly used?**

A:

```
==
!=
<
>
<=
>=
```

**Q48: Why are conditionals important?**

A: They let your program react differently in different situations.

**Q49: Can I have more than one condition?**

A: Yes.

```csharp
if (age >= 18 && hasID)
```

**Q50: What is the easiest way to think about an if statement?**

A: Think of it like asking a yes-or-no question before doing something.

</details>

<details>
<summary><h3>Random Numbers</h3></summary>

**Q51: What is a random number?**

A: It is a number chosen unpredictably from a range.

**Q52: When should I use random numbers?**

A: Use them for games, simulations, dice rolls, or random choices.

**Q53: How do I create a Random object?**

A:

```csharp
Random random = new Random();
```

**Q54: How do I generate a random number?**

A:

```csharp
int number = random.Next(1, 11);
```

**Q55: What does Next(1, 11) mean?**

A: It generates numbers from 1 through 10.

**Q56: Why do I create the Random object only once?**

A: Reusing one Random object gives better random results.

**Q57: Can I generate random decimal numbers?**

A: Yes.

```csharp
double value = random.NextDouble();
```

**Q58: How can I simulate rolling a die?**

A:

```csharp
int roll = random.Next(1, 7);
```

**Q59: How can I randomly choose between true and false?**

A:

```csharp
bool result = random.Next(2) == 0;
```

**Q60: Why are random numbers useful?**

A: They make programs less predictable and more interesting by creating different results each time.

</details>
</details>

<details>
<summary><h2>Code Syntax</h2></summary>

<details>
<summary><h3>Variables & Constants</h3></summary>

**Q1: I want to store a player's name in my program.**

A:

```csharp
string playerName = "John";
```

**Q2: I want to store a score that will change during the game.**

A:

```csharp
int score = 0;
```

**Q3: I want to store the value of PI that should never change.**

A:

```csharp
const double PI = 3.14159;
```

**Q4: I want to store whether a player is alive or dead.**

A:

```csharp
bool isAlive = true;
```

**Q5: I want to store a fixed game title.**

A:

```csharp
const string gameTitle = "Space Battle";
```

**Q6: I want to increase a score by 10.**

A:

```csharp
score += 10;
```

**Q7: I want to reset a score to zero.**

A:

```csharp
score = 0;
```

**Q8: I want to store a character grade.**

A:

```csharp
char grade = 'A';
```

**Q9: I want to store a decimal health value.**

A:

```csharp
double health = 75.5;
```

**Q10: I want to update a player's name.**

A:

```csharp
playerName = "Alex";
```

</details>

<details>
<summary><h3>Data Types</h3></summary>

**Q11: I want to store whole numbers only.**

A:

```csharp
int level = 1;
```

**Q12: I want to store text input from a user.**

A:

```csharp
string input = Console.ReadLine();
```

**Q13: I want to store a yes/no value.**

A:

```csharp
bool hasKey = false;
```

**Q14: I want to store a single letter.**

A:

```csharp
char initial = 'B';
```

**Q15: I want to store a precise price value.**

A:

```csharp
double price = 19.99;
```

**Q16: I want to convert string input into an integer.**

A:

```csharp
int age = int.Parse(Console.ReadLine());
```

**Q17: I want to store a large number safely.**

A:

```csharp
long distance = 1000000000;
```

**Q18: I want to store a floating-point calculation result.**

A:

```csharp
float temperature = 36.6f;
```

**Q19: I want to store multiple words in a variable.**

A:

```csharp
string message = "Hello World";
```

**Q20: I want to store whether a door is open or closed.**

A:

```csharp
bool isOpen = true;
```

</details>

<details>
<summary><h3>Input / Output (CLI)</h3></summary>

**Q21: I want to print a message to the console.**

A:

```csharp
Console.WriteLine("Hello Player");
```

**Q22: I want to print without going to a new line.**

A:

```csharp
Console.Write("Enter name: ");
```

**Q23: I want to ask the user for their name.**

A:

```csharp
string name = Console.ReadLine();
```

**Q24: I want to display the user's name.**

A:

```csharp
Console.WriteLine(name);
```

**Q25: I want to combine text and variables in output.**

A:

```csharp
Console.WriteLine("Hello " + name);
```

**Q26: I want to convert input to a number.**

A:

```csharp
int number = int.Parse(Console.ReadLine());
```

**Q27: I want to show a score to the user.**

A:

```csharp
Console.WriteLine("Score: " + score);
```

**Q28: I want to pause the program until input is entered.**

A:

```csharp
Console.ReadLine();
```

**Q29: I want to display multiple lines of text.**

A:

```csharp
Console.WriteLine("Line 1\nLine 2");
```

**Q30: I want to clear the console screen.**

A:

```csharp
Console.Clear();
```

</details>

<details>
<summary><h3>Basic Math Operations</h3></summary>

**Q31: I want to add two numbers.**

A:

```csharp
int result = a + b;
```

**Q32: I want to subtract two numbers.**

A:

```csharp
int result = a - b;
```

**Q33: I want to multiply two numbers.**

A:

```csharp
int result = a * b;
```

**Q34: I want to divide two numbers.**

A:

```csharp
int result = a / b;
```

**Q35: I want to find remainder of division.**

A:

```csharp
int remainder = a % b;
```

**Q36: I want to increase a variable by 1.**

A:

```csharp
count++;
```

**Q37: I want to decrease a variable by 1.**

A:

```csharp
count--;
```

**Q38: I want to add 5 to a score.**

A:

```csharp
score += 5;
```

**Q39: I want to double a value.**

A:

```csharp
value *= 2;
```

**Q40: I want to average two numbers.**

A:

```csharp
double avg = (a + b) / 2.0;
```

</details>

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

**Q41: I want to check if a player is old enough.**

A:

```csharp
if (age >= 18)
{
    Console.WriteLine("Allowed");
}
```

**Q42: I want to block underage users.**

A:

```csharp
if (age < 18)
{
    Console.WriteLine("Blocked");
}
```

**Q43: I want to handle both pass and fail.**

A:

```csharp
if (score >= 50)
{
    Console.WriteLine("Pass");
}
else
{
    Console.WriteLine("Fail");
}
```

**Q44: I want to check if a number is equal to 10.**

A:

```csharp
if (number == 10)
{
    Console.WriteLine("Match");
}
```

**Q45: I want to check if two conditions are true.**

A:

```csharp
if (hasKey && doorLocked)
{
    Console.WriteLine("Open door");
}
```

**Q46: I want to check if either condition is true.**

A:

```csharp
if (isAdmin || isModerator)
{
    Console.WriteLine("Access granted");
}
```

**Q47: I want to check if a number is not equal to 0.**

A:

```csharp
if (number != 0)
{
    Console.WriteLine("Valid");
}
```

**Q48: I want to handle multiple conditions.**

A:

```csharp
if (score > 80)
{
    Console.WriteLine("A");
}
else if (score > 50)
{
    Console.WriteLine("B");
}
else
{
    Console.WriteLine("C");
}
```

**Q49: I want to check if a user is logged in.**

A:

```csharp
if (isLoggedIn)
{
    Console.WriteLine("Welcome");
}
```

**Q50: I want to stop invalid input.**

A:

```csharp
if (input == "")
{
    Console.WriteLine("Invalid input");
}
```

</details>

<details>
<summary><h3>Random Numbers</h3></summary>

**Q51: I want to generate a random number between 1 and 10.**

A:

```csharp
Random rand = new Random();
int number = rand.Next(1, 11);
```

**Q52: I want to simulate a dice roll.**

A:

```csharp
Random rand = new Random();
int roll = rand.Next(1, 7);
```

**Q53: I want to randomly pick true or false.**

A:

```csharp
Random rand = new Random();
bool result = rand.Next(2) == 0;
```

**Q54: I want to generate a random decimal.**

A:

```csharp
Random rand = new Random();
double value = rand.NextDouble();
```

**Q55: I want to randomly pick a number between 50 and 100.**

A:

```csharp
Random rand = new Random();
int value = rand.Next(50, 101);
```

**Q56: I want to simulate a coin flip.**

A:

```csharp
Random rand = new Random();
string flip = rand.Next(2) == 0 ? "Heads" : "Tails";
```

**Q57: I want to randomly increase score by 1 or 2.**

A:

```csharp
Random rand = new Random();
score += rand.Next(1, 3);
```

**Q58: I want to randomly choose a name.**

A:

```csharp
string[] names = { "Alex", "Sam", "Jordan" };
Random rand = new Random();
string pick = names[rand.Next(names.Length)];
```

**Q59: I want to generate a random damage value.**

A:

```csharp
Random rand = new Random();
int damage = rand.Next(5, 16);
```

**Q60: I want to randomly decide if an attack hits.**

A:

```csharp
Random rand = new Random();
bool hit = rand.Next(100) < 75;
```

</details>
</details>

<details>
<summary><h2>Flowcharts + Key</h2></summary>

<details>
<summary><h3>Flowchart Shape Key</h3></summary>

| Text shape | Actual flowchart shape | Purpose |
| --- | --- | --- |
| `([ START / END ])` | **Oval / Terminator** | Beginning or ending |
| `[ Process ]` | **Rectangle** | Calculation, assignment, setup |
| `[/ Input /]` | **Parallelogram** | User input or displayed output |
| `{ Decision? }` | **Diamond** | Condition / branching |
| `↓` | **Arrow** | Direction of execution |

</details>

<details>
<summary><h3>Project 1: Simple CLI Calculator</h3></summary>

#### Text-based flowchart

```
             ([ START ])
                  |
                  ↓
       [/ Ask for first number /]
                  |
                  ↓
       [/ Read first number /]
                  |
                  ↓
       [ Convert input to integer ]
                  |
                  ↓
       [/ Ask for second number /]
                  |
                  ↓
       [/ Read second number /]
                  |
                  ↓
       [ Convert input to integer ]
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
       [/ Display addition result /]
                  |
                  ↓
       [/ Display subtraction result /]
                  |
                  ↓
       [/ Display multiplication result /]
                  |
                  ↓
       [/ Display division result /]
                  |
                  ↓
             ([ END ])
```

#### Shape breakdown

- Start → **Terminator**
- Ask for number → **Input/Output**
- Read input → **Input/Output**
- Convert to integer → **Process**
- Calculate operations → **Process**
- Display results → **Input/Output**
- End → **Terminator**

**Important:** The actual C# code does not separately "convert" the value after reading it—the `int.Parse()` happens as part of the input statement. The separate conversion box is useful for teaching the underlying logic.

</details>

<details>
<summary><h3>Project 2: Number Guessing Game</h3></summary>

#### Text-based flowchart

```
             ([ START ])
                  |
                  ↓
       [ Create Random generator ]
                  |
                  ↓
       [ Generate secret number
             between 1-10 ]
                  |
                  ↓
       [/ Ask user for guess /]
                  |
                  ↓
       [/ Read user's guess /]
                  |
                  ↓
       [ Convert guess to integer ]
                  |
                  ↓
          { Guess == Secret? }
             /           \
           YES            NO
            |              |
            ↓              ↓
   [/ Display "Correct!" /] [/ Display "Wrong!" /]
            |              |
            |              ↓
            |       [/ Display secret number /]
            |              |
            └───────┬──────┘
                    ↓
                ([ END ])
```

#### Shape breakdown

- Create `Random` → **Process**
- Generate secret → **Process**
- Ask/read guess → **Input/Output**
- Convert guess → **Process**
- Compare values → **Decision**
- Display result → **Input/Output**
- End → **Terminator**

#### Core logic

```
              Guess == Secret?
                 /       \
              YES         NO
               ↓           ↓
            Correct       Wrong
```

This is your basic **if/else** flow.

</details>

<details>
<summary><h3>Project 3: Login Check System</h3></summary>

#### Text-based flowchart

```
             ([ START ])
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
       { Username correct
         AND
         Password correct? }
             /          \
           YES           NO
            |             |
            ↓             ↓
 [/ Display "Access     [/ Display "Access
       Granted" /]            Denied" /]
            |             |
            └──────┬──────┘
                   ↓
               ([ END ])
```

#### Shape breakdown

- Store credentials → **Process**
- Ask/read username → **Input/Output**
- Ask/read password → **Input/Output**
- Check credentials → **Decision**
- Display access result → **Input/Output**
- End → **Terminator**

#### Core logic

The diamond represents **two conditions combined with `&&`**:

```
user == correctUser
        AND
pass == correctPass
        ↓
     Decision
```

Both must be true to reach **Access Granted**.

</details>

<details>
<summary><h3>Project 4: Simple Grade Calculator</h3></summary>

This one is the most useful example for teaching **else-if chains**.

#### Text-based flowchart

```
             ([ START ])
                  |
                  ↓
          [/ Ask for score /]
                  |
                  ↓
          [/ Read score /]
                  |
                  ↓
       [ Convert score to integer ]
                  |
                  ↓
             { score >= 90? }
              /           \
            YES            NO
             |              |
             ↓              ↓
       [/ Grade: A /]   { score >= 80? }
             |            /          \
             |          YES           NO
             |           |             |
             |           ↓             ↓
             |      [/ Grade: B /] { score >= 70? }
             |                         /        \
             |                       YES         NO
             |                        |           |
             |                        ↓           ↓
             |                  [/ Grade: C /] { score >= 60? }
             |                                    /      \
             |                                  YES       NO
             |                                   |         |
             |                                   ↓         ↓
             |                             [/ Grade: D /] [/ Grade: F /]
             |                                   |         |
             └───────────────────┬───────────────┴─────────┘
                                 ↓
                            ([ END ])
```

#### Shape breakdown

- Ask for score → **Input/Output**
- Read score → **Input/Output**
- Convert score → **Process**
- Every `score >= X` → **Decision**
- Display grade → **Input/Output**
- End → **Terminator**

#### The logic structure

```
score >= 90?
   ├── YES → A
   └── NO
        ↓
     score >= 80?
        ├── YES → B
        └── NO
             ↓
          score >= 70?
             ├── YES → C
             └── NO
                  ↓
               score >= 60?
                  ├── YES → D
                  └── NO → F
```

This is a great visual example of how:

```
ifelseifelseifelseifelse
```

creates a **decision chain**.

</details>

<details>
<summary><h3>Project 5: Dice Battle Simulator</h3></summary>

#### Text-based flowchart

```
             ([ START ])
                  |
                  ↓
       [ Create Random generator ]
                  |
                  ↓
       [ Roll Player 1
         between 1-6 ]
                  |
                  ↓
       [ Roll Player 2
         between 1-6 ]
                  |
                  ↓
       [/ Display Player 1 roll /]
                  |
                  ↓
       [/ Display Player 2 roll /]
                  |
                  ↓
          { Player 1 > Player 2? }
             /             \
           YES              NO
            |                |
            ↓                ↓
 [/ Display "Player 1    { Player 2 > Player 1? }
       wins!" /]            /              \
            |              YES              NO
            |               |                |
            |               ↓                ↓
            |       [/ Display "Player 2  [/ Display
            |             wins!" /]        "It's a tie!" /]
            |               |                |
            └───────┬───────┴────────────────┘
                    ↓
                ([ END ])
```

#### Shape breakdown

- Create random generator → **Process**
- Roll dice → **Process**
- Display rolls → **Input/Output**
- Compare Player 1 vs Player 2 → **Decision**
- Compare Player 2 vs Player 1 → **Decision**
- Display winner/tie → **Input/Output**
- End → **Terminator**

#### Core logic

```
          Player 1 > Player 2?
             /          \
           YES           NO
            ↓             ↓
       Player 1 wins   Player 2 > Player 1?
                            /       \
                          YES        NO
                           ↓          ↓
                      Player 2 wins  Tie
```

</details>
</details>

<details>
<summary><h2>Sample Projects</h2></summary>

<details>
<summary><h3>Project 1: Simple CLI Calculator</h3></summary>

#### What it does

Takes two numbers from the user and performs basic math operations.

#### Step-by-step

1. Ask user for first number
2. Ask user for second number
3. Convert input to integers
4. Add, subtract, multiply, divide
5. Display results

```csharp
using System;

class Program
{
    static void Main()
    {
        // Step 1: Ask user for first number
        Console.Write("Enter first number: ");
        int num1 = int.Parse(Console.ReadLine());

        // Step 2: Ask user for second number
        Console.Write("Enter second number: ");
        int num2 = int.Parse(Console.ReadLine());

        // Step 3: Perform calculations
        int add = num1 + num2;
        int subtract = num1 - num2;
        int multiply = num1 * num2;
        int divide = num1 / num2;

        // Step 4: Display results
        Console.WriteLine("Add: " + add);
        Console.WriteLine("Subtract: " + subtract);
        Console.WriteLine("Multiply: " + multiply);
        Console.WriteLine("Divide: " + divide);
    }
}
```

</details>

<details>
<summary><h3>Project 2: Number Guessing Game</h3></summary>

#### What it does

User guesses a random number between 1 and 10.

#### Step-by-step

1. Generate random number
2. Ask user for guess
3. Compare guess to number
4. Tell user if correct or wrong

```csharp
using System;

class Program
{
    static void Main()
    {
        // Step 1: Generate random number
        Random rand = new Random();
        int secret = rand.Next(1, 11);

        // Step 2: Ask user for guess
        Console.Write("Guess a number (1-10): ");
        int guess = int.Parse(Console.ReadLine());

        // Step 3: Compare values
        if (guess == secret)
        {
            Console.WriteLine("Correct!");
        }
        else
        {
            Console.WriteLine("Wrong! The number was " + secret);
        }
    }
}
```

</details>

<details>
<summary><h3>Project 3: Login Check System</h3></summary>

#### What it does

Checks username and password input.

#### Step-by-step

1. Store correct username/password
2. Ask user for input
3. Compare values
4. Show access result

```csharp
using System;

class Program
{
    static void Main()
    {
        // Step 1: Stored credentials
        string correctUser = "admin";
        string correctPass = "1234";

        // Step 2: Ask user for input
        Console.Write("Enter username: ");
        string user = Console.ReadLine();

        Console.Write("Enter password: ");
        string pass = Console.ReadLine();

        // Step 3: Compare credentials
        if (user == correctUser && pass == correctPass)
        {
            Console.WriteLine("Access Granted");
        }
        else
        {
            Console.WriteLine("Access Denied");
        }
    }
}
```

</details>

<details>
<summary><h3>Project 4: Simple Grade Calculator</h3></summary>

#### What it does

Converts numeric score into a letter grade.

#### Step-by-step

1. Ask user for score
2. Convert input to number
3. Check score ranges
4. Output grade

```csharp
using System;

class Program
{
    static void Main()
    {
        // Step 1: Ask for score
        Console.Write("Enter score (0-100): ");
        int score = int.Parse(Console.ReadLine());

        // Step 2: Determine grade
        if (score >= 90)
        {
            Console.WriteLine("Grade: A");
        }
        else if (score >= 80)
        {
            Console.WriteLine("Grade: B");
        }
        else if (score >= 70)
        {
            Console.WriteLine("Grade: C");
        }
        else if (score >= 60)
        {
            Console.WriteLine("Grade: D");
        }
        else
        {
            Console.WriteLine("Grade: F");
        }
    }
}
```

</details>

<details>
<summary><h3>Project 5: Dice Battle Simulator</h3></summary>

#### What it does

Two players roll dice; highest roll wins.

#### Step-by-step

1. Create random generator
2. Roll dice for player 1
3. Roll dice for player 2
4. Compare results
5. Declare winner

```csharp
using System;

class Program
{
    static void Main()
    {
        // Step 1: Create random generator
        Random rand = new Random();

        // Step 2: Player 1 roll
        int player1 = rand.Next(1, 7);

        // Step 3: Player 2 roll
        int player2 = rand.Next(1, 7);

        // Step 4: Show results
        Console.WriteLine("Player 1 rolled: " + player1);
        Console.WriteLine("Player 2 rolled: " + player2);

        // Step 5: Determine winner
        if (player1 > player2)
        {
            Console.WriteLine("Player 1 wins!");
        }
        else if (player2 > player1)
        {
            Console.WriteLine("Player 2 wins!");
        }
        else
        {
            Console.WriteLine("It's a tie!");
        }
    }
}
```

</details>
</details>