<details>
<summary><h1>Coding Basics/White Belt/C++ + CLI</h1></summary>

💡 Tip: Click the arrows next to each heading to expand or collapse the content underneath.

<details>
<summary><h2>Key Concepts</h2></summary>

<details>
<summary><h3>Variables & Constants</h3></summary>

**Q1: What is a variable in C++?**

A: A variable is a named container that stores data your program can change.

**Q2: When should I use a variable?**

A: When the value needs to change while the program runs.

**Q3: How do I create a variable in C++?**

A:

```cpp
int score = 10;
```

**Q4: What is a constant in C++?**

A: A constant is a value that cannot change after it is set.

**Q5: How do I create a constant?**

A:

```cpp
const int MAX = 100;
```

**Q6: When should I use a constant?**

A: When the value should never change, like limits or fixed settings.

**Q7: Why use variables instead of fixed values?**

A: So your program can change and adapt.

**Q8: What does const do?**

A: It locks a value so it cannot be modified.

**Q9: Can variables change in C++?**

A: Yes, unless marked const.

**Q10: Why are variables important?**

A: They let programs remember and update information.

</details>

---

<details>
<summary><h3>Data Types</h3></summary>

**Q11: What is a data type?**

A: It tells C++ what kind of value is stored.

**Q12: What is an int?**

A:

```cpp
int age = 20;
```

**Q13: What is a double?**

A:

```cpp
double price = 4.99;
```

**Q14: What is a string?**

A:

```cpp
#include <string>
std::string name = "Alex";
```

**Q15: What is a bool?**

A:

```cpp
bool isAlive = true;
```

**Q16: When should I use int vs double?**

A: int for whole numbers, double for decimals.

**Q17: Why do data types matter?**

A: They prevent incorrect operations.

**Q18: What is char?**

A:

```cpp
char grade = 'A';
```

**Q19: Can types be mixed?**

A: Yes, but it may require conversion.

**Q20: Why choose correct types?**

A: To keep programs predictable and safe.

</details>

---

<details>
<summary><h3>Input / Output (CLI)</h3></summary>

**Q21: How do I print text in C++?**

A:

```cpp
#include <iostream>
std::cout << "Hello";
```

**Q22: What is output?**

A: Information shown to the user.

**Q23: What is input?**

A: Data the user types in the terminal.

**Q24: How do I read input?**

A:

```cpp
int age;
std::cin >> age;
```

**Q25: Why use std::cin?**

A: It allows keyboard input.

**Q26: How do I read a string with spaces?**

A:

```cpp
std::getline(std::cin, name);
```

**Q27: Why use std::cout?**

A: It prints output to the terminal.

**Q28: What is the << operator?**

A: It sends data to output.

**Q29: What is the >> operator?**

A: It takes input from the user.

**Q30: Why use CLI input/output?**

A: It makes programs interactive.

</details>

---

<details>
<summary><h3>Basic Math Operations</h3></summary>

**Q31: How do I add numbers in C++?**

A:

```cpp
int result = a + b;
```

**Q32: How do I subtract?**

A:

```cpp
int result = a - b;
```

**Q33: How do I multiply?**

A:

```cpp
int result = a * b;
```

**Q34: How do I divide?**

A:

```cpp
int result = a / b;
```

**Q35: What is modulus?**

A:

```cpp
int r = a % b;
```

**Q36: When should I use modulus?**

A: For remainder checks like even/odd.

**Q37: What happens in integer division?**

A: Decimals are removed.

**Q38: How to get decimal division?**

A:

```cpp
double result = (double)a / b;
```

**Q39: Why store math results?**

A: So they can be reused.

**Q40: Why is math important?**

A: Many programs rely on calculations.

</details>

---

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

**Q41: What is an if statement?**

A: A decision tool in code.

**Q42: When should I use if?**

A: When something depends on a condition.

**Q43: How do I write an if statement?**

A:

```cpp
if (age >= 18) {
    std::cout << "Adult";
}
```

**Q44: What is else?**

A: What happens when if is false.

**Q45: How do I use else?**

A:

```cpp
if (score >= 50) {
    std::cout << "Pass";
} else {
    std::cout << "Fail";
}
```

**Q46: What is a condition?**

A: A true or false question.

**Q47: What operators are used in conditions?**

A:

```
== != < > <= >=
```

**Q48: Why use conditions?**

A: To control program behavior.

**Q49: Can I check multiple conditions?**

A:

```cpp
if (age > 18 && hasID)
```

**Q50: What does && mean?**

A: Both conditions must be true.

</details>

---

<details>
<summary><h3>Random Numbers</h3></summary>

**Q51: How do I generate random numbers in C++?**

A:

```cpp
#include <cstdlib>
#include <ctime>

std::srand(time(0));
int num = std::rand() % 10 + 1;
```

**Q52: What does rand() do?**

A: Generates a random number.

**Q53: Why use srand(time(0))?**

A: To make numbers different each run.

**Q54: How do I get 1–6 random?**

A:

```cpp
int roll = std::rand() % 6 + 1;
```

**Q55: When should I use random numbers?**

A: Games and simulations.

**Q56: Why is rand() limited?**

A: It produces predictable sequences without seeding.

**Q57: How do I generate true randomness?**

A: Use modern C++ `<random>` library.

**Q58: How do I pick true/false randomly?**

A:

```cpp
bool b = std::rand() % 2;
```

**Q59: How do I randomize decisions?**

A:

```cpp
if (std::rand() % 100 < 50)
```

**Q60: Why are random numbers useful?**

A: They make programs unpredictable and dynamic.

</details>

</details>

<details>
<summary><h2>Code Syntax</h2></summary>

<details>
<summary><h3>Variables & Constants</h3></summary>

**Q1: I want to store a player's name.**

A:

```cpp
std::string playerName = "Alex";
```

**Q2: I want to store a score that changes.**

A:

```cpp
int score = 0;
```

**Q3: I want to store a constant max value.**

A:

```cpp
const int MAX_SCORE = 100;
```

**Q4: I want to increase score by 10.**

A:

```cpp
score += 10;
```

**Q5: I want to reset a score.**

A:

```cpp
score = 0;
```

**Q6: I want to store player health.**

A:

```cpp
int health = 100;
```

**Q7: I want to store true/false state.**

A:

```cpp
bool isAlive = true;
```

**Q8: I want to store a decimal value.**

A:

```cpp
double price = 19.99;
```

**Q9: I want to store a single character.**

A:

```cpp
char grade = 'A';
```

**Q10: I want to update a variable value.**

A:

```cpp
playerName = "Jordan";
```

</details>

---

<details>
<summary><h3>Input / Output (CLI)</h3></summary>

**Q11: I want to print text to terminal.**

A:

```cpp
std::cout << "Hello World";
```

**Q12: I want to read a number from user.**

A:

```cpp
int age;
std::cin >> age;
```

**Q13: I want to read a string with spaces.**

A:

```cpp
std::getline(std::cin, playerName);
```

**Q14: I want to print a variable.**

A:

```cpp
std::cout << score;
```

**Q15: I want to print text and variable together.**

A:

```cpp
std::cout << "Score: " << score;
```

**Q16: I want to ask for two inputs.**

A:

```cpp
int a, b;
std::cin >> a >> b;
```

**Q17: I want to print a new line.**

A:

```cpp
std::cout << "\n";
```

**Q18: I want to display a welcome message.**

A:

```cpp
std::cout << "Welcome!\n";
```

**Q19: I want to pause program for input.**

A:

```cpp
std::cin.get();
```

**Q20: I want to display both values.**

A:

```cpp
std::cout << a << " " << b;
```

</details>

---

<details>
<summary><h3>Basic Math Operations</h3></summary>

**Q21: I want to add two numbers.**

A:

```cpp
int result = a + b;
```

**Q22: I want to subtract.**

A:

```cpp
int result = a - b;
```

**Q23: I want to multiply.**

A:

```cpp
int result = a * b;
```

**Q24: I want to divide.**

A:

```cpp
int result = a / b;
```

**Q25: I want remainder.**

A:

```cpp
int r = a % b;
```

**Q26: I want to increase value by 1.**

A:

```cpp
score++;
```

**Q27: I want to decrease value by 1.**

A:

```cpp
score--;
```

**Q28: I want to double a value.**

A:

```cpp
value *= 2;
```

**Q29: I want to average two numbers.**

A:

```cpp
double avg = (a + b) / 2.0;
```

**Q30: I want to calculate total cost.**

A:

```cpp
double total = price * quantity;
```

</details>

---

<details>
<summary><h3>Conditionals (if / else)</h3></summary>

**Q31: I want to check if user is adult.**

A:

```cpp
if (age >= 18) {
    std::cout << "Adult";
}
```

**Q32: I want to block minors.**

A:

```cpp
if (age < 18) {
    std::cout << "Blocked";
}
```

**Q33: I want pass/fail check.**

A:

```cpp
if (score >= 50) {
    std::cout << "Pass";
} else {
    std::cout << "Fail";
}
```

**Q34: I want equality check.**

A:

```cpp
if (a == b) {
    std::cout << "Equal";
}
```

**Q35: I want not equal check.**

A:

```cpp
if (a != b) {
    std::cout << "Not equal";
}
```

**Q36: I want greater than check.**

A:

```cpp
if (score > 80) {
    std::cout << "High score";
}
```

**Q37: I want multiple conditions (AND).**

A:

```cpp
if (age > 18 && hasID) {
    std::cout << "Allowed";
}
```

**Q38: I want OR condition.**

A:

```cpp
if (isAdmin || isMod) {
    std::cout << "Access granted";
}
```

**Q39: I want grade system.**

A:

```cpp
if (score >= 90) {
    std::cout << "A";
} else if (score >= 80) {
    std::cout << "B";
} else {
    std::cout << "C";
}
```

**Q40: I want to check empty input.**

A:

```cpp
if (input.empty()) {
    std::cout << "Invalid";
}
```

</details>

---

<details>
<summary><h3>Random Numbers</h3></summary>

**Q41: I want random number 1–10.**

A:

```cpp
#include <cstdlib>
#include <ctime>

std::srand(time(0));
int num = std::rand() % 10 + 1;
```

**Q42: I want dice roll.**

A:

```cpp
int roll = std::rand() % 6 + 1;
```

**Q43: I want random true/false.**

A:

```cpp
bool b = std::rand() % 2;
```

**Q44: I want random damage.**

A:

```cpp
int damage = std::rand() % 10 + 5;
```

**Q45: I want random chance check.**

A:

```cpp
if (std::rand() % 100 < 50)
```

**Q46: I want random 50–100 number.**

A:

```cpp
int num = std::rand() % 51 + 50;
```

**Q47: I want random array selection.**

A:

```cpp
std::string names[] = {"A", "B", "C"};
std::string pick = names[std::rand() % 3];
```

**Q48: I want critical hit chance.**

A:

```cpp
if (std::rand() % 100 < 25)
```

**Q49: I want random decision output.**

A:

```cpp
std::cout << (std::rand() % 2 ? "Yes" : "No");
```

**Q50: I want random event trigger.**

A:

```cpp
if (std::rand() % 100 < 10) {
    std::cout << "Event!";
}
```

</details>

---

<details>
<summary><h3>Mixed CLI Logic</h3></summary>

**Q51: I want greet user by name.**

A:

```cpp
std::cout << "Hello " << name;
```

**Q52: I want add two inputs directly.**

A:

```cpp
int sum = a + b;
```

**Q53: I want check positive number.**

A:

```cpp
if (num > 0) {
    std::cout << "Positive";
}
```

**Q54: I want prevent divide by zero.**

A:

```cpp
if (b != 0) {
    std::cout << a / b;
}
```

**Q55: I want limit score max to 100.**

A:

```cpp
if (score > 100) score = 100;
```

**Q56: I want show name and score.**

A:

```cpp
std::cout << name << ": " << score;
```

**Q57: I want login check.**

A:

```cpp
if (user == "admin" && pass == "1234")
```

**Q58: I want check empty string.**

A:

```cpp
if (input.empty())
```

**Q59: I want compare max value.**

A:

```cpp
std::cout << std::max(a, b);
```

**Q60: I want trigger rare event.**

A:

```cpp
if (std::rand() % 100 < 5) {
    std::cout << "Rare event!";
}
```

</details>

</details>

<details>
<summary><h2>Flowcharts + Key</h2></summary>

<details>
<summary><h3>Flowchart Shape Key</h3></summary>

| Shape | Meaning | Used for |
| --- | --- | --- |
| `([ START / END ])` | **Oval / Terminator** | Program start or end |
| `[ Process ]` | **Rectangle** | Calculations, assignments, setup, generating values |
| `[/ Input / Output /]` | **Parallelogram** | User input and displayed output |
| `{ Condition? }` | **Diamond** | `if`, comparisons, decisions |
| `↓` | **Arrow** | Direction of program flow |

</details>

---

<details>
<summary><h3>Project 1: CLI Calculator</h3></summary>

**Text-Based Flowchart**

```
([ START ])
     ↓
[ Include libraries / Set up program ]
     ↓
[/ Display "Enter first number:" /]
     ↓
[/ Read integer a /]
     ↓
[/ Display "Enter second number:" /]
     ↓
[/ Read integer b /]
     ↓
[ Calculate add = a + b ]
     ↓
[ Calculate sub = a - b ]
     ↓
[ Calculate mul = a * b ]
     ↓
{ b != 0? }
  ↙       ↘
YES       NO
 ↓         ↓
[ div =    [ div =
 a / b ]    0 ]
  ↘       ↙
    ↓
[/ Display Add result /]
    ↓
[/ Display Subtract result /]
    ↓
[/ Display Multiply result /]
    ↓
[/ Display Divide result /]
    ↓
([ END ])
```

**Flowchart Shapes**

- **START** → Oval
- **Include libraries / setup** → Rectangle
- **Ask for first number** → Parallelogram
- **Read `a`** → Parallelogram
- **Ask for second number** → Parallelogram
- **Read `b`** → Parallelogram
- **Calculate addition** → Rectangle
- **Calculate subtraction** → Rectangle
- **Calculate multiplication** → Rectangle
- **`b != 0?`** → Diamond
- **`div = a / b`** → Rectangle
- **`div = 0`** → Rectangle
- **Display results** → Parallelograms
- **END** → Oval

**Core logic:** Input → Calculate → Protect against division by zero → Output.

</details>

---

<details>
<summary><h3>Project 2: Number Guessing Game</h3></summary>

**Text-Based Flowchart**

```
([ START ])
     ↓
[ Include libraries / Set up random generator ]
     ↓
[ Generate secret number from 1–10 ]
     ↓
[/ Display "Guess a number (1-10):" /]
     ↓
[/ Read guess /]
     ↓
{ guess == secret? }
   ↙          ↘
 YES          NO
  ↓            ↓
[/ Display      [/ Display
 "Correct!" /]   "Wrong! It was secret" /]
   ↘          ↙
      ↓
   ([ END ])
```

**Flowchart Shapes**

- **START** → Oval
- **Setup random generator** → Rectangle
- **Generate secret number** → Rectangle
- **Ask for guess** → Parallelogram
- **Read `guess`** → Parallelogram
- **`guess == secret?`** → Diamond
- **Display Correct** → Parallelogram
- **Display Wrong + secret** → Parallelogram
- **END** → Oval

**Core logic:** Generate → Input → Compare → Branch → Output.

</details>

---

<details>
<summary><h3>Project 3: Simple Login System</h3></summary>

**Text-Based Flowchart**

```
([ START ])
     ↓
[ Store correctUser = "admin" ]
     ↓
[ Store correctPass = "1234" ]
     ↓
[/ Display "Username:" /]
     ↓
[/ Read user /]
     ↓
[/ Display "Password:" /]
     ↓
[/ Read pass /]
     ↓
{ user == correctUser
  AND
  pass == correctPass? }
      ↙             ↘
    YES             NO
     ↓               ↓
[/ Display          [/ Display
 "Access             "Access
 Granted" /]         Denied" /]
      ↘             ↙
         ↓
      ([ END ])
```

**Flowchart Shapes**

- **START** → Oval
- **Store correct username** → Rectangle
- **Store correct password** → Rectangle
- **Display Username prompt** → Parallelogram
- **Read username** → Parallelogram
- **Display Password prompt** → Parallelogram
- **Read password** → Parallelogram
- **Username AND password correct?** → Diamond
- **Access Granted** → Parallelogram
- **Access Denied** → Parallelogram
- **END** → Oval

**Important Logic**

```
Username correct ──┐
                   ├── AND ──> Access Granted
Password correct ──┘
```

Both conditions must be **true**.

</details>

---

<details>
<summary><h3>Project 4: Grade Calculator</h3></summary>

This one is different because it has a **decision chain**.

**Text-Based Flowchart**

```
([ START ])
     ↓
[/ Display "Enter score:" /]
     ↓
[/ Read score /]
     ↓
{ score >= 90? }
   ↙          ↘
 YES          NO
  ↓            ↓
[/ Output A /] { score >= 80? }
                ↙          ↘
              YES          NO
               ↓            ↓
          [/ Output B /] { score >= 70? }
                           ↙          ↘
                         YES          NO
                          ↓            ↓
                     [/ Output C /] { score >= 60? }
                                      ↙          ↘
                                    YES          NO
                                     ↓            ↓
                                [/ Output D /] [/ Output F /]
                                     ↘          ↙
                                       ↓
                                    ([ END ])
```

**Flowchart Shapes**

- **START** → Oval
- **Display score prompt** → Parallelogram
- **Read score** → Parallelogram
- **`score >= 90?`** → Diamond
- **Output A** → Parallelogram
- **`score >= 80?`** → Diamond
- **Output B** → Parallelogram
- **`score >= 70?`** → Diamond
- **Output C** → Parallelogram
- **`score >= 60?`** → Diamond
- **Output D** → Parallelogram
- **Output F** → Parallelogram
- **END** → Oval

**Core Logic**

```
90+ → A
 ↓
80+ → B
 ↓
70+ → C
 ↓
60+ → D
 ↓
<60 → F
```

The important concept here is that each failed condition moves to the **next condition**.

</details>

---

<details>
<summary><h3>Project 5: Dice Battle Simulator</h3></summary>

**Text-Based Flowchart**

```
([ START ])
     ↓
[ Include libraries / Set up random generator ]
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
           "Player      "Tie!" /]
           2 Wins!" /]
              ↘         ↙
                 ↓
              ([ END ])
```

**Flowchart Shapes**

- **START** → Oval
- **Setup random generator** → Rectangle
- **Generate Player 1 roll** → Rectangle
- **Generate Player 2 roll** → Rectangle
- **Display Player 1 roll** → Parallelogram
- **Display Player 2 roll** → Parallelogram
- **`p1 > p2?`** → Diamond
- **Player 1 Wins** → Parallelogram
- **`p2 > p1?`** → Diamond
- **Player 2 Wins** → Parallelogram
- **Tie** → Parallelogram
- **END** → Oval

</details>

---

<details>
<summary><h3>C++ Master Flowchart</h3></summary>

All five projects can be reduced to this universal programming structure:

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
               ([ END ])
```

**The C++ concepts these five projects progressively introduce**

| Project | Main concept |
| --- | --- |
| **1. Calculator** | Variables, input, arithmetic, ternary decision |
| **2. Guessing Game** | Random numbers + comparison |
| **3. Login** | Strings + `&&` / compound conditions |
| **4. Grade Calculator** | `if / else if / else` decision chains |
| **5. Dice Battle** | Random numbers + multiple branches |

</details>

</details>

<details>
<summary><h2>Sample Projects</h2></summary>

<details>
<summary><h3>Project 1: CLI Calculator</h3></summary>

**What it does**

Takes two numbers and performs basic math operations.

**Steps**

1. Ask user for two numbers
2. Store inputs
3. Perform math
4. Display results

```cpp
#include <iostream>
using namespace std;

int main() {

    // Step 1: Ask for first number
    cout << "Enter first number: ";
    int a;
    cin >> a;

    // Step 2: Ask for second number
    cout << "Enter second number: ";
    int b;
    cin >> b;

    // Step 3: Perform calculations
    int add = a + b;
    int sub = a - b;
    int mul = a * b;
    int div = (b != 0) ? (a / b) : 0;

    // Step 4: Display results
    cout << "Add: " << add << endl;
    cout << "Subtract: " << sub << endl;
    cout << "Multiply: " << mul << endl;
    cout << "Divide: " << div << endl;

    return 0;
}
```

</details>

---

<details>
<summary><h3>Project 2: Number Guessing Game</h3></summary>

**What it does**

User guesses a random number from 1–10.

**Steps**

1. Generate random number
2. Ask user guess
3. Compare values
4. Output result

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;

int main() {

    srand(time(0));

    // Step 1: Generate random number
    int secret = rand() % 10 + 1;

    // Step 2: Ask user guess
    cout << "Guess a number (1-10): ";
    int guess;
    cin >> guess;

    // Step 3: Compare
    if (guess == secret) {
        cout << "Correct!" << endl;
    }
    else {
        cout << "Wrong! It was " << secret << endl;
    }

    return 0;
}
```

</details>

---

<details>
<summary><h3>Project 3: Simple Login System</h3></summary>

**What it does**

Checks username and password in CLI.

**Steps**

1. Store correct credentials
2. Ask user input
3. Compare values
4. Show result

```cpp
#include <iostream>
using namespace std;

int main() {

    // Step 1: Stored credentials
    string correctUser = "admin";
    string correctPass = "1234";

    // Step 2: Ask user input
    string user, pass;

    cout << "Username: ";
    cin >> user;

    cout << "Password: ";
    cin >> pass;

    // Step 3: Compare
    if (user == correctUser && pass == correctPass) {
        cout << "Access Granted" << endl;
    }
    else {
        cout << "Access Denied" << endl;
    }

    return 0;
}
```

</details>

---

<details>
<summary><h3>Project 4: Grade Calculator</h3></summary>

**What it does**

Turns numeric score into letter grade.

**Steps**

1. Get score
2. Check ranges
3. Print grade

```cpp
#include <iostream>
using namespace std;

int main() {

    // Step 1: Get input
    cout << "Enter score: ";
    int score;
    cin >> score;

    // Step 2: Determine grade
    if (score >= 90) {
        cout << "A" << endl;
    }
    else if (score >= 80) {
        cout << "B" << endl;
    }
    else if (score >= 70) {
        cout << "C" << endl;
    }
    else if (score >= 60) {
        cout << "D" << endl;
    }
    else {
        cout << "F" << endl;
    }

    return 0;
}
```

</details>

---

<details>
<summary><h3>Project 5: Dice Battle Simulator</h3></summary>

**What it does**

Two players roll dice and highest wins.

**Steps**

1. Seed random
2. Generate rolls
3. Compare
4. Print winner

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;

int main() {

    srand(time(0));

    // Step 1: Player 1 roll
    int p1 = rand() % 6 + 1;

    // Step 2: Player 2 roll
    int p2 = rand() % 6 + 1;

    // Step 3: Display rolls
    cout << "Player 1: " << p1 << endl;
    cout << "Player 2: " << p2 << endl;

    // Step 4: Compare results
    if (p1 > p2) {
        cout << "Player 1 Wins!" << endl;
    }
    else if (p2 > p1) {
        cout << "Player 2 Wins!" << endl;
    }
    else {
        cout << "Tie!" << endl;
    }

    return 0;
}
```

</details>

</details>