
<details>
<summary><h1>Coding Basics/White Belt/.bat + CLI</h1></summary>

💡 Tip: Click the arrows next to each heading to expand or collapse the content underneath.

<details>
<summary><h2>Key Concepts</h2></summary>

<details>
<summary><h3>Variables & “Constants” (Batch-style variables)</h3></summary>

**Q1: What is a variable in a .bat file?**

A: A variable is a named placeholder that stores text or values.

```bash
set name=Alex
```

**Q2: When should I use a variable in batch?**

A: When you need to reuse or change a value during the script.

**Q3: How do I create a variable?**

A:

```bash
set score=10
```

**Q4: How do I use a variable?**

A:

```bash
echo %score%
```

**Q5: Can variables change in .bat?**

A: Yes, by using set again.

```bash
set score=20
```

**Q6: What is a “constant” in .bat?**

A: Batch doesn’t have real constants, but you simulate one by not changing it.

**Q7: How do I simulate a constant?**

A:

```bash
set MAX=100
```

**Q8: Why use variables instead of writing values directly?**

A: So you can change values in one place.

**Q9: What does %variable% mean?**

A: It tells batch to insert the variable’s value.

**Q10: Why are variables important in batch?**

A: They let scripts remember and reuse data.

</details>

---

<details>
<summary><h3>Data Types (Simple CLI meaning)</h3></summary>

**Q11: What data types exist in .bat?**

A: Mostly text (strings), but numbers and booleans are treated as text.

**Q12: How do I store a number?**

A:

```bash
set num=5
```

**Q13: How do I store text?**

A:

```bash
set name=Hello
```

**Q14: How do I store true/false?**

A:

```bash
set isOn=true
```

**Q15: Why does batch treat everything like text?**

A: Because it is a scripting language, not a compiled one.

**Q16: How do I convert string to number behavior?**

A: Batch does math automatically in SET /A.

**Q17: Why does data type matter less in batch?**

A: Because batch is loosely typed.

**Q18: What is a “value” in batch?**

A: Anything stored after = in a variable.

**Q19: Can variables store spaces?**

A:

```bash
set name=John Doe
```

**Q20: Why use quotes carefully?**

A: Spaces can break commands if not handled properly.

</details>

---

<details>
<summary><h3>Input / Output (CLI)</h3></summary>

**Q21: How do I print text in batch?**

A:

```bash
echo Hello World
```

**Q22: How do I print a variable?**

A:

```bash
echo %name%
```

**Q23: How do I take user input?**

A:

```bash
set /p name=Enter your name:
```

**Q24: Why use set /p?**

A: It pauses and reads user input.

**Q25: How do I display a message?**

A:

```bash
echo Welcome!
```

**Q26: How do I clear the screen?**

A:

```bash
cls
```

**Q27: Why use echo?**

A: It outputs text to the terminal.

**Q28: How do I print blank lines?**

A:

```bash
echo.
```

**Q29: How do I combine text and variables?**

A:

```bash
echo Hello %name%
```

**Q30: Why is CLI output important?**

A: It shows results of your script.

</details>

---

<details>
<summary><h3>Basic Math Operations</h3></summary>

**Q31: How do I add numbers in batch?**

A:

```bash
set /a result=5+3
```

**Q32: How do I subtract?**

A:

```bash
set /a result=10-4
```

**Q33: How do I multiply?**

A:

```bash
set /a result=3*3
```

**Q34: How do I divide?**

A:

```bash
set /a result=10/2
```

**Q35: What is /a?**

A: It tells batch to perform arithmetic.

**Q36: Can batch do decimals?**

A: Not well; it uses integer math.

**Q37: What is modulus?**

A:

```bash
set /a result=10%%3
```

**Q38: Why use %% instead of %?**

A: Because % is reserved for variables.

**Q39: How do I increase a number?**

A:

```bash
set /a score+=1
```

**Q40: Why use math in scripts?**

A: For counters, timers, and logic.

</details>

---

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

**Q41: What is an if statement in batch?**

A: A decision command.

**Q42: How do I use if?**

A:

```bash
if %score%==10 echo Perfect
```

**Q43: How do I use if/else?**

A:

```bash
if %score%==10 (
    echo Perfect
) else (
    echo Try again
)
```

**Q44: What does == mean?**

A: It compares values.

**Q45: When should I use if?**

A: When something depends on a condition.

**Q46: How do I check not equal?**

A:

```bash
if not %score%==10 echo Wrong
```

**Q47: Why use parentheses in batch if?**

A: To group commands.

**Q48: How do I check empty input?**

A:

```bash
if "%name%"=="" echo Empty
```

**Q49: What does “not” mean?**

A: It reverses the condition.

**Q50: Why are conditionals important?**

A: They make scripts smart and dynamic.

</details>

---

<details>
<summary><h3>Random Numbers (Batch-style simulation)</h3></summary>

**Q51: Does batch have real random?**

A: Yes, via %RANDOM%.

**Q52: How do I get a random number?**

A:

```bash
echo %RANDOM%
```

**Q53: How do I get 1–10 random?**

A:

```bash
set /a num=%RANDOM% %% 10 + 1
```

**Q54: What does %RANDOM% do?**

A: Generates a random number.

**Q55: Why use modulus with RANDOM?**

A: To limit range.

**Q56: How do I simulate dice roll?**

A:

```bash
set /a roll=%RANDOM% %% 6 + 1
```

**Q57: How do I simulate a coin flip?**

A:

```bash
set /a flip=%RANDOM% %% 2
```

**Q58: When should I use random?**

A: Games, simulations, random behavior.

**Q59: Why is RANDOM useful?**

A: It adds unpredictability.

**Q60: How do I make a random decision?**

A:

```bash
if %RANDOM% LSS 16384 echo Yes
```

</details>
</details>

<details>
<summary><h2>Code Syntax</h2></summary>

<details>
<summary><h3>Variables & Basic Setup</h3></summary>

**Q1: I want to store a username.**

A:

```bash
set username=Alex
```

**Q2: I want to store a score.**

A:

```bash
set score=0
```

**Q3: I want to update a score by adding 10.**

A:

```bash
set /a score+=10
```

**Q4: I want to reset a score to zero.**

A:

```bash
set score=0
```

**Q5: I want to store a max value.**

A:

```bash
set MAX=100
```

**Q6: I want to store player health.**

A:

```bash
set health=100
```

**Q7: I want to store a boolean state.**

A:

```bash
set alive=true
```

**Q8: I want to overwrite a variable.**

A:

```bash
set username=Jordan
```

**Q9: I want to store a level number.**

A:

```bash
set level=1
```

**Q10: I want to double a value.**

A:

```bash
set /a score*=2
```

</details>

---

<details>
<summary><h3>Input / Output (CLI)</h3></summary>

**Q11: I want to print text.**

A:

```bash
echo Hello World
```

**Q12: I want to print a variable.**

A:

```bash
echo %username%
```

**Q13: I want to ask for user input.**

A:

```bash
set /p name=Enter your name:
```

**Q14: I want to display a welcome message.**

A:

```bash
echo Welcome %name%
```

**Q15: I want to clear the screen.**

A:

```bash
cls
```

**Q16: I want to print a blank line.**

A:

```bash
echo.
```

**Q17: I want to show score output.**

A:

```bash
echo Score: %score%
```

**Q18: I want to display multiple variables.**

A:

```bash
echo %username% %score%
```

**Q19: I want to pause the program.**

A:

```bash
pause
```

**Q20: I want to hide commands from output.**

A:

```bash
@echo off
```

</details>

---

<details>
<summary><h3>Math Operations</h3></summary>

**Q21: I want to add two numbers.**

A:

```bash
set /a result=5+3
```

**Q22: I want to subtract numbers.**

A:

```bash
set /a result=10-4
```

**Q23: I want to multiply numbers.**

A:

```bash
set /a result=3*3
```

**Q24: I want to divide numbers.**

A:

```bash
set /a result=10/2
```

**Q25: I want remainder.**

A:

```bash
set /a result=10%%3
```

**Q26: I want to increase score by 1.**

A:

```bash
set /a score+=1
```

**Q27: I want to decrease score.**

A:

```bash
set /a score-=1
```

**Q28: I want to calculate total price.**

A:

```bash
set /a total=price*quantity
```

**Q29: I want to calculate sum of inputs.**

A:

```bash
set /a sum=a+b
```

**Q30: I want to square a number.**

A:

```bash
set /a result=num*num
```

</details>

---

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

**Q31: I want to check if score equals 10.**

A:

```bash
if %score%==10 echo Perfect
```

**Q32: I want to check if score is greater than 50.**

A:

```bash
if %score% GTR 50 echo High Score
```

**Q33: I want to check if score is less than 50.**

A:

```bash
if %score% LSS 50 echo Low Score
```

**Q34: I want to run code if user is admin.**

A:

```bash
if %role%==admin echo Access Granted
```

**Q35: I want to handle pass/fail.**

A:

```bash
if %score% GEQ 50 (
    echo Pass
) else (
    echo Fail
)
```

**Q36: I want to check empty input.**

A:

```bash
if "%name%"=="" echo Empty input
```

**Q37: I want to check not equal.**

A:

```bash
if not %score%==10 echo Not Perfect
```

**Q38: I want to run multiple commands in IF.**

A:

```bash
if %score% GTR 50 (
    echo Good
    echo Keep going
)
```

**Q39: I want to check two conditions (AND logic).**

A:

```bash
if %score% GTR 50 if %health% GTR 0 echo Alive
```

**Q40: I want to block invalid input.**

A:

```bash
if "%input%"=="" echo Invalid
```

</details>

---

<details>
<summary><h3>Random Numbers (%RANDOM%)</h3></summary>

**Q41: I want a random number.**

A:

```bash
echo %RANDOM%
```

**Q42: I want 1–10 random number.**

A:

```bash
set /a num=%RANDOM% %% 10 + 1
```

**Q43: I want dice roll.**

A:

```bash
set /a roll=%RANDOM% %% 6 + 1
```

**Q44: I want coin flip.**

A:

```bash
set /a flip=%RANDOM% %% 2
```

**Q45: I want random damage.**

A:

```bash
set /a damage=%RANDOM% %% 10 + 5
```

**Q46: I want random chance check.**

A:

```bash
if %RANDOM% LSS 16384 echo Success
```

**Q47: I want random 50–100 range.**

A:

```bash
set /a num=%RANDOM% %% 51 + 50
```

**Q48: I want random event trigger.**

A:

```bash
if %RANDOM% LSS 5000 echo Event Triggered
```

**Q49: I want random yes/no output.**

A:

```bash
if %RANDOM% LSS 16384 (echo Yes) else (echo No)
```

**Q50: I want random selection between two actions.**

A:

```bash
if %RANDOM% LSS 16384 echo Action A
if %RANDOM% GEQ 16384 echo Action B
```

</details>

---

<details>
<summary><h3>Mixed CLI Logic</h3></summary>

**Q51: I want to greet user by name.**

A:

```bash
echo Hello %name%
```

**Q52: I want to add two numbers from variables.**

A:

```bash
set /a sum=%a%+%b%
```

**Q53: I want to limit score to 100.**

A:

```bash
if %score% GTR 100 set score=100
```

**Q54: I want to check if player is alive.**

A:

```bash
if %alive%==true echo You are alive
```

**Q55: I want to show stats.**

A:

```bash
echo Name: %name% Score: %score%
```

**Q56: I want to stop execution if input is empty.**

A:

```bash
if "%input%"=="" exit
```

**Q57: I want to compare two variables.**

A:

```bash
if %a%==%b% echo Equal
```

**Q58: I want to simulate leveling up.**

A:

```bash
set /a level+=1
```

**Q59: I want to show final result.**

A:

```bash
echo Final Score: %score%
```

**Q60: I want to trigger rare event.**

A:

```bash
if %RANDOM% LSS 1000 echo Rare Event Triggered
```

</details>
</details>

<details>
<summary><h2>Flowcharts + Key</h2></summary>

<details>
<summary><h3>Flowchart Shape Key</h3></summary>

| Shape | Meaning | Batch File examples |
| --- | --- | --- |
| `([ START / END ])` | **Oval / Terminator** | Start/end of `.bat` program |
| `[ Process ]` | **Rectangle** | `set`, `set /a`, setup, calculations |
| `[/ Input / Output /]` | **Parallelogram** | `set /p`, `echo`, `pause` |
| `{ Condition? }` | **Diamond** | `if` / `else` decisions |
| `↓` | **Arrow** | Direction of execution |

</details>

---

<details>
<summary><h3>Project 1: CLI Calculator — Batch File</h3></summary>

**Text-Based Flowchart**

```
([ START ])
    ↓
[ Turn echo off: @echo off ]
    ↓
[/ Ask for first number /]
    ↓
[/ Read and store a /]
    ↓
[/ Ask for second number /]
    ↓
[/ Read and store b /]
    ↓
[ Calculate add = a + b ]
    ↓
[ Calculate sub = a - b ]
    ↓
[ Calculate mul = a * b ]
    ↓
[ Calculate div = a / b ]
    ↓
[/ Display Addition result /]
    ↓
[/ Display Subtraction result /]
    ↓
[/ Display Multiplication result /]
    ↓
[/ Display Division result /]
    ↓
[/ Pause /]
    ↓
([ END ])
```

**Flowchart Shapes**

- **START** → Oval
- **`@echo off`** → Rectangle
- **Ask for first number** → Parallelogram
- **Read/store `a`** → Parallelogram
- **Ask for second number** → Parallelogram
- **Read/store `b`** → Parallelogram
- **`add = a+b`** → Rectangle
- **`sub = a-b`** → Rectangle
- **`mul = a*b`** → Rectangle
- **`div = a/b`** → Rectangle
- **Display results** → Parallelograms
- **`pause`** → Parallelogram
- **END** → Oval

**Core Pattern**

```
INPUT → STORE → CALCULATE → OUTPUT
```

</details>

---

<details>
<summary><h3>Project 2: Number Guessing Game</h3></summary>

**Text-Based Flowchart**

```
([ START ])
    ↓
[ Turn echo off: @echo off ]
    ↓
[ Generate random secret number 1–10 ]
    ↓
[/ Ask user for guess /]
    ↓
[/ Read and store guess /]
    ↓
{ guess == secret? }
    ↙          ↘
  YES          NO
   ↓            ↓
[/ Display     [/ Display
 "Correct!" /]  "Wrong! It was secret" /]
    ↘          ↙
       ↓
   [/ Pause /]
       ↓
   ([ END ])
```

**Flowchart Shapes**

- **START** → Oval
- **`@echo off`** → Rectangle
- **Generate random number** → Rectangle
- **Ask for guess** → Parallelogram
- **Read/store `guess`** → Parallelogram
- **`guess == secret?`** → Diamond
- **Display Correct** → Parallelogram
- **Display Wrong + secret** → Parallelogram
- **Pause** → Parallelogram
- **END** → Oval

**Core Pattern**

```
GENERATE RANDOM VALUE
       ↓
     INPUT
       ↓
   COMPARE
    ↙    ↘
  YES    NO
   ↓      ↓
OUTPUT   OUTPUT
    ↘    ↙
      END
```

</details>

---

<details>
<summary><h3>Project 3: Simple Login System</h3></summary>

**Text-Based Flowchart**

```
([ START ])
    ↓
[ Turn echo off: @echo off ]
    ↓
[ Store user = "admin" ]
    ↓
[ Store pass = "1234" ]
    ↓
[/ Ask for username /]
    ↓
[/ Read/store inputUser /]
    ↓
[/ Ask for password /]
    ↓
[/ Read/store inputPass /]
    ↓
{ inputUser == user
 AND
 inputPass == pass? }
      ↙             ↘
    YES             NO
     ↓               ↓
[/ Display          [/ Display
 "Access             "Access
 Granted" /]         Denied" /]
      ↘             ↙
         ↓
     [/ Pause /]
         ↓
     ([ END ])
```

**Flowchart Shapes**

- **START** → Oval
- **`@echo off`** → Rectangle
- **Store username** → Rectangle
- **Store password** → Rectangle
- **Ask for username** → Parallelogram
- **Read username** → Parallelogram
- **Ask for password** → Parallelogram
- **Read password** → Parallelogram
- **Credentials correct?** → Diamond
- **Access Granted** → Parallelogram
- **Access Denied** → Parallelogram
- **Pause** → Parallelogram
- **END** → Oval

**Core Logic**

```
Username correct ──┐
                   ├── AND ──> DECISION
Password correct ──┘
                       ↓
                Granted / Denied
```

The important Batch concept here is that the nested `if` statements effectively create an **AND condition**.

</details>

---

<details>
<summary><h3>Project 4: Score Tracker</h3></summary>

This one introduces a **value modification + upper-limit decision**.

**Text-Based Flowchart**

```
([ START ])
    ↓
[ Turn echo off: @echo off ]
    ↓
[/ Ask for starting score /]
    ↓
[/ Read/store score /]
    ↓
[ Generate random points from 1–20 ]
    ↓
[ Add random points to score ]
    ↓
{ score > 100? }
    ↙          ↘
  YES          NO
   ↓            ↓
[ Set score     [ Keep score
  = 100 ]         unchanged ]
    ↘          ↙
       ↓
[/ Display final score /]
       ↓
[/ Pause /]
       ↓
   ([ END ])
```

**Flowchart Shapes**

- **START** → Oval
- **`@echo off`** → Rectangle
- **Ask for starting score** → Parallelogram
- **Read/store score** → Parallelogram
- **Generate random points** → Rectangle
- **Add points to score** → Rectangle
- **`score > 100?`** → Diamond
- **Set `score = 100`** → Rectangle
- **Keep score unchanged** → Rectangle
- **Display final score** → Parallelogram
- **Pause** → Parallelogram
- **END** → Oval

**Core Logic**

```
STARTING SCORE
     ↓
RANDOM POINTS
     ↓
ADD POINTS
     ↓
SCORE > 100?
  ↙       ↘
YES       NO
 ↓         ↓
CAP 100   KEEP SCORE
  ↘       ↙
  DISPLAY
     ↓
    END
```

This is a good example of a **constraint/cap**:

```
score = score + random points

IF score > 100
   score = 100
```

</details>

---

<details>
<summary><h3>Project 5: Dice Battle Simulator</h3></summary>

**Text-Based Flowchart**

```
([ START ])
    ↓
[ Turn echo off: @echo off ]
    ↓
[ Generate Player 1 roll: 1–6 ]
    ↓
[ Generate Player 2 roll: 1–6 ]
    ↓
[/ Display Player 1 roll /]
    ↓
[/ Display Player 2 roll /]
    ↓
{ p1 > p2? }
   ↙          ↘
 YES          NO
  ↓            ↓
[/ Display    { p2 > p1? }
 "Player 1     ↙       ↘
 Wins!" /]   YES       NO
              ↓         ↓
         [/ Display   [/ Display
           "Player      "It's a
           2 Wins!" /]   Tie!" /]
              ↘         ↙
                 ↓
             [/ Pause /]
                 ↓
             ([ END ])
```

**Flowchart Shapes**

- **START** → Oval
- **`@echo off`** → Rectangle
- **Generate Player 1 roll** → Rectangle
- **Generate Player 2 roll** → Rectangle
- **Display Player 1 roll** → Parallelogram
- **Display Player 2 roll** → Parallelogram
- **`p1 > p2?`** → Diamond
- **Player 1 Wins** → Parallelogram
- **`p2 > p1?`** → Diamond
- **Player 2 Wins** → Parallelogram
- **Tie** → Parallelogram
- **Pause** → Parallelogram
- **END** → Oval

</details>

---

<details>
<summary><h3>Batch File Master Flowchart</h3></summary>

Your five projects fit into the same overall programming model you've been using across languages:

```
             ([ START ])
                  ↓
            [ PROGRAM SETUP ]
                  ↓
             [/ INPUT /]
                  ↓
             [ PROCESS ]
                  ↓
           { DECISION? }
             ↙       ↘
           YES       NO
            ↓         ↓
       [ PROCESS ] [ PROCESS ]
            ↘       ↙
               ↓
            [/ OUTPUT /]
               ↓
            [/ PAUSE /]
               ↓
             ([ END ])
```

**What Batch File adds to your belt progression**

| Project | Main concept |
| --- | --- |
| **1. Calculator** | Variables + arithmetic + input/output |
| **2. Guessing Game** | Random values + comparison |
| **3. Login** | Strings + nested `if` + AND logic |
| **4. Score Tracker** | Variable modification + constraints |
| **5. Dice Battle** | Random values + multiple decisions |

</details>
</details>

<details>
<summary><h2>Sample Projects</h2></summary>

<details>
<summary><h3>Project 1: CLI Calculator (Batch File)</h3></summary>

**What it does**

Takes two numbers from the user and performs basic math operations.

**Steps**

1. Turn echo off
2. Ask for first number
3. Ask for second number
4. Perform math operations
5. Display results

```bash
@echo off

:: Step 1: Ask for first number
set /p a=Enter first number:

:: Step 2: Ask for second number
set /p b=Enter second number:

:: Step 3: Perform calculations
set /a add=a+b
set /a sub=a-b
set /a mul=a*b
set /a div=a/b

:: Step 4: Display results
echo Addition: %add%
echo Subtraction: %sub%
echo Multiplication: %mul%
echo Division: %div%

pause
```

</details>

---

<details>
<summary><h3>Project 2: Number Guessing Game</h3></summary>

**What it does**

User guesses a random number between 1–10.

**Steps**

1. Generate random number
2. Ask user for guess
3. Compare values
4. Show result

```bash
@echo off

:: Step 1: Generate random number (1–10)
set /a secret=%RANDOM% %% 10 + 1

:: Step 2: Ask user for guess
set /p guess=Guess a number (1-10):

:: Step 3: Compare values
if %guess%==%secret% (
    echo Correct!
) else (
    echo Wrong! It was %secret%
)

pause
```

</details>

---

<details>
<summary><h3>Project 3: Simple Login System</h3></summary>

**What it does**

Checks username and password.

**Steps**

1. Store correct credentials
2. Ask user input
3. Compare values
4. Show result

```bash
@echo off

:: Step 1: Store credentials
set user=admin
set pass=1234

:: Step 2: Get input
set /p inputUser=Username:
set /p inputPass=Password:

:: Step 3: Compare
if "%inputUser%"=="%user%" if "%inputPass%"=="%pass%" (
    echo Access Granted
) else (
    echo Access Denied
)

pause
```

</details>

---

<details>
<summary><h3>Project 4: Score Tracker</h3></summary>

**What it does**

Adds points and limits max score to 100.

**Steps**

1. Ask starting score
2. Add random points
3. Limit score
4. Display result

```bash
@echo off

:: Step 1: Get starting score
set /p score=Enter starting score:

:: Step 2: Add random points (1–20)
set /a score+=%RANDOM% %% 20 + 1

:: Step 3: Cap score at 100
if %score% GTR 100 set score=100

:: Step 4: Display final score
echo Final Score: %score%

pause
```

</details>

---

<details>
<summary><h3>Project 5: Dice Battle Simulator</h3></summary>

**What it does**

Two players roll dice; highest wins.

**Steps**

1. Generate Player 1 roll
2. Generate Player 2 roll
3. Compare results
4. Display winner

```bash
@echo off

:: Step 1: Player 1 roll (1–6)
set /a p1=%RANDOM% %% 6 + 1

:: Step 2: Player 2 roll (1–6)
set /a p2=%RANDOM% %% 6 + 1

:: Step 3: Show rolls
echo Player 1 rolled: %p1%
echo Player 2 rolled: %p2%

:: Step 4: Compare results
if %p1% GTR %p2% (
    echo Player 1 Wins!
) else if %p2% GTR %p1% (
    echo Player 2 Wins!
) else (
    echo It's a Tie!
)

pause
```

</details>
</details>
