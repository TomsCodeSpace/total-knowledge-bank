<details>
<summary><h1>Coding Basics/White Belt/C# + GUI (WinForms)</h1></summary>

💡 Tip: Click the arrows next to each heading to expand or collapse the content underneath.

<details>
<summary><h2>Key Concepts</h2></summary>

<details>
<summary><h3>Variables & Constants (WinForms Basics)</h3></summary>

**Q1: What is a variable in WinForms?**

A: A variable stores data the app uses, like text from a textbox or a score.

**Q2: When should I use a variable in a WinForms app?**

A: When you need to store user input or update values on the form.

**Q3: How do I store textbox input in a variable?**

A:

```csharp
string name = textBox1.Text;
```

**Q4: Why do I use variables in GUI apps?**

A: Because UI controls don’t “remember” values unless you store them.

**Q5: What is a constant in WinForms?**

A: A value that never changes, like a fixed tax rate.

**Q6: How do I create a constant in WinForms?**

A:

```csharp
const double TAX_RATE = 0.07;
```

**Q7: When should I use constants in GUI apps?**

A: When a value is reused but should never change.

**Q8: Can I store button text in a variable?**

A:

```csharp
string buttonText = button1.Text;
```

**Q9: How do I change a label using a variable?**

A:

```csharp
label1.Text = name;
```

**Q10: Why separate UI values into variables?**

A: It makes logic easier to manage than reading controls repeatedly.

</details>

<details>
<summary><h3>Data Types (WinForms Context)</h3></summary>

**Q11: What data type is textbox input?**

A: It is always a string.

**Q12: How do I convert textbox text to an integer?**

A:

```csharp
int age = int.Parse(textBox1.Text);
```

**Q13: Why do I convert strings in WinForms?**

A: Because math and logic need numbers, not text.

**Q14: What is a bool used for in GUI apps?**

A: It stores true/false states like checkbox status.

**Q15: How do I read a checkbox value?**

A:

```csharp
bool isChecked = checkBox1.Checked;
```

**Q16: What is a double used for?**

A: Decimal values like price or measurements.

**Q17: How do I store a decimal from input?**

A:

```csharp
double price = double.Parse(textBox1.Text);
```

**Q18: Why is string the default UI type?**

A: Because all UI input starts as text.

**Q19: What is the safest number type for UI?**

A: int or double depending on decimals.

**Q20: Why do types matter in GUI apps?**

A: They prevent wrong operations like adding text instead of numbers.

</details>

<details>
<summary><h3>Input / Output (WinForms Controls)</h3></summary>

**Q21: What is output in WinForms?**

A: Displaying data on labels, message boxes, or textboxes.

**Q22: How do I show output in a label?**

A:

```csharp
label1.Text = "Hello";
```

**Q23: How do I show a popup message?**

A:

```csharp
MessageBox.Show("Hello!");
```

**Q24: What is input in WinForms?**

A: Data the user enters into controls like textboxes.

**Q25: How do I get input from a textbox?**

A:

```csharp
string input = textBox1.Text;
```

**Q26: Why use MessageBox instead of console?**

A: GUI apps don’t use a terminal for interaction.

**Q27: How do I clear a textbox?**

A:

```csharp
textBox1.Clear();
```

**Q28: How do I update UI after button click?**

A:

```csharp
label1.Text = textBox1.Text;
```

**Q29: Why do buttons trigger input handling?**

A: Because GUI apps run on events, not loops.

**Q30: What is event-driven input?**

A: Code runs only when user clicks or interacts.

</details>

<details>
<summary><h3>Basic Math Operations (WinForms)</h3></summary>

**Q31: How do I add two textbox numbers?**

A:

```csharp
int result = int.Parse(textBox1.Text) + int.Parse(textBox2.Text);
```

**Q32: How do I show math result in label?**

A:

```csharp
label1.Text = result.ToString();
```

**Q33: Why do I convert textbox values first?**

A: Because math cannot be done on strings.

**Q34: How do I subtract in WinForms?**

A:

```csharp
int result = a - b;
```

**Q35: How do I multiply user inputs?**

A:

```csharp
int result = a * b;
```

**Q36: How do I divide safely?**

A:

```csharp
if (b != 0) result = a / b;
```

**Q37: Why check for zero before dividing?**

A: To prevent crashes.

**Q38: How do I calculate total price?**

A:

```csharp
double total = price * quantity;
```

**Q39: How do I increase score in GUI?**

A:

```csharp
score += 1;
```

**Q40: Why store math results in variables?**

A: So UI can reuse and display them easily.

</details>

<details>
<summary><h3>Conditionals (if/else in WinForms)</h3></summary>

**Q41: How do I check if textbox is empty?**

A:

```csharp
if (textBox1.Text == "")
```

**Q42: Why check empty input?**

A: To prevent invalid calculations.

**Q43: How do I show message if input is invalid?**

A:

```csharp
MessageBox.Show("Invalid input");
```

**Q44: How do I check checkbox condition?**

A:

```csharp
if (checkBox1.Checked)
```

**Q45: When should I use if statements in GUI apps?**

A: When user input changes behavior.

**Q46: How do I check age restriction?**

A:

```csharp
if (age >= 18)
```

**Q47: How do I handle multiple conditions?**

A:

```csharp
if (score > 90) label1.Text = "A";
```

**Q48: Why are conditionals important in UI?**

A: They control app behavior based on user input.

**Q49: How do I disable a button based on condition?**

A:

```csharp
button1.Enabled = false;
```

**Q50: What is UI logic?**

A: Decisions made based on user interaction.

</details>

<details>
<summary><h3>Random Numbers (WinForms)</h3></summary>

**Q51: How do I generate a random number in WinForms?**

A:

```csharp
Random rand = new Random();
int number = rand.Next(1, 11);
```

**Q52: Why use random numbers in GUI apps?**

A: For games, simulations, and unpredictable results.

**Q53: How do I show random number in label?**

A:

```csharp
label1.Text = number.ToString();
```

**Q54: How do I roll a dice in WinForms?**

A:

```csharp
int roll = rand.Next(1, 7);
```

**Q55: How do I generate random button behavior?**

A:

```csharp
button1.Enabled = rand.Next(2) == 0;
```

**Q56: How do I randomize background color (logic only)?**

A:

```csharp
int value = rand.Next(256);
```

**Q57: Why create Random once?**

A: To avoid repeating patterns.

**Q58: How do I pick random text?**

A:

```csharp
string[] options = { "A", "B", "C" };
string pick = options[rand.Next(options.Length)];
```

**Q59: How do I simulate a coin flip?**

A:

```csharp
string result = rand.Next(2) == 0 ? "Heads" : "Tails";
```

**Q60: Why are random features useful in WinForms?**

A: They make apps interactive and game-like instead of predictable.

</details>
</details>

<details>
<summary><h2>Code Syntax</h2></summary>

<details>
<summary><h3>Variables & Constants (WinForms)</h3></summary>

**Q1: I want to store a user's name from a textbox.**

A:

```csharp
string name = textBox1.Text;
```

**Q2: I want to store a score that updates when a button is clicked.**

A:

```csharp
int score = 0;
```

**Q3: I want to store a fixed tax rate for calculations.**

A:

```csharp
const double TAX_RATE = 0.07;
```

**Q4: I want to store whether a checkbox is checked.**

A:

```csharp
bool isChecked = checkBox1.Checked;
```

**Q5: I want to update a label with a variable value.**

A:

```csharp
label1.Text = score.ToString();
```

**Q6: I want to increase score when a button is clicked.**

A:

```csharp
score++;
```

**Q7: I want to reset score when clicking a reset button.**

A:

```csharp
score = 0;
label1.Text = score.ToString();
```

**Q8: I want to store textbox input for later use.**

A:

```csharp
string input = textBox1.Text;
```

**Q9: I want to store a product name from input.**

A:

```csharp
string productName = textBoxProduct.Text;
```

**Q10: I want to store a constant app title.**

A:

```csharp
const string APP_NAME = "Calculator App";
```

</details>

<details>
<summary><h3>Data Types (WinForms)</h3></summary>

**Q11: I want to convert textbox text into an integer.**

A:

```csharp
int number = int.Parse(textBox1.Text);
```

**Q12: I want to convert textbox text into a decimal value.**

A:

```csharp
double value = double.Parse(textBox1.Text);
```

**Q13: I want to store true/false from a checkbox.**

A:

```csharp
bool enabled = checkBox1.Checked;
```

**Q14: I want to store a single character input.**

A:

```csharp
char letter = textBox1.Text[0];
```

**Q15: I want to display number as text in a label.**

A:

```csharp
label1.Text = number.ToString();
```

**Q16: I want to store large numbers.**

A:

```csharp
long bigNumber = long.Parse(textBox1.Text);
```

**Q17: I want to store floating point temperature.**

A:

```csharp
float temp = float.Parse(textBox1.Text);
```

**Q18: I want to combine text and number for display.**

A:

```csharp
label1.Text = "Score: " + score;
```

**Q19: I want to safely store user input text.**

A:

```csharp
string text = textBox1.Text;
```

**Q20: I want to convert boolean logic into UI decision.**

A:

```csharp
button1.Enabled = isChecked;
```

</details>

<details>
<summary><h3>Input / Output (WinForms)</h3></summary>

**Q21: I want to display a popup message.**

A:

```csharp
MessageBox.Show("Hello!");
```

**Q22: I want to show textbox input in a label.**

A:

```csharp
label1.Text = textBox1.Text;
```

**Q23: I want to clear a textbox when button is clicked.**

A:

```csharp
textBox1.Clear();
```

**Q24: I want to get user input from textbox.**

A:

```csharp
string input = textBox1.Text;
```

**Q25: I want to show calculation result in UI.**

A:

```csharp
label1.Text = result.ToString();
```

**Q26: I want to print debug info to console (WinForms debugging).**

A:

```csharp
Console.WriteLine("Debug info");
```

**Q27: I want to disable a button after clicking it.**

A:

```csharp
button1.Enabled = false;
```

**Q28: I want to enable a button when input is valid.**

A:

```csharp
button1.Enabled = true;
```

**Q29: I want to update label when checkbox changes.**

A:

```csharp
label1.Text = checkBox1.Checked.ToString();
```

**Q30: I want to display multiple values in UI.**

A:

```csharp
label1.Text = "Name: " + name + " Score: " + score;
```

</details>

<details>
<summary><h3>Basic Math Operations (WinForms)</h3></summary>

**Q31: I want to add two textbox numbers.**

A:

```csharp
int result = int.Parse(textBox1.Text) + int.Parse(textBox2.Text);
```

**Q32: I want to subtract two numbers from input.**

A:

```csharp
int result = int.Parse(textBox1.Text) - int.Parse(textBox2.Text);
```

**Q33: I want to multiply user inputs.**

A:

```csharp
int result = int.Parse(textBox1.Text) * int.Parse(textBox2.Text);
```

**Q34: I want to divide two textbox values.**

A:

```csharp
int result = int.Parse(textBox1.Text) / int.Parse(textBox2.Text);
```

**Q35: I want to prevent division by zero.**

A:

```csharp
if (b != 0)
{
    result = a / b;
}
```

**Q36: I want to calculate total price.**

A:

```csharp
double total = double.Parse(textBox1.Text) * double.Parse(textBox2.Text);
```

**Q37: I want to increase score by 5.**

A:

```csharp
score += 5;
```

**Q38: I want to decrease health.**

A:

```csharp
health -= 10;
```

**Q39: I want to calculate remainder in UI app.**

A:

```csharp
int result = a % b;
```

**Q40: I want to average two numbers.**

A:

```csharp
double avg = (a + b) / 2.0;
```

</details>

<details>
<summary><h3>Conditionals (if / else in WinForms)</h3></summary>

**Q41: I want to check if textbox is empty.**

A:

```csharp
if (textBox1.Text == "")
{
    MessageBox.Show("Empty input");
}
```

**Q42: I want to validate age input.**

A:

```csharp
if (int.Parse(textBox1.Text) >= 18)
{
    MessageBox.Show("Allowed");
}
```

**Q43: I want to block invalid input.**

A:

```csharp
if (textBox1.Text == "")
{
    button1.Enabled = false;
}
```

**Q44: I want to show pass/fail result.**

A:

```csharp
if (score >= 50)
{
    label1.Text = "Pass";
}
else
{
    label1.Text = "Fail";
}
```

**Q45: I want to check checkbox before enabling button.**

A:

```csharp
button1.Enabled = checkBox1.Checked;
```

**Q46: I want to check admin access.**

A:

```csharp
if (textBoxUser.Text == "admin")
{
    MessageBox.Show("Access granted");
}
```

**Q47: I want to handle multiple score levels.**

A:

```csharp
if (score > 80)
    label1.Text = "A";
else if (score > 50)
    label1.Text = "B";
else
    label1.Text = "C";
```

**Q48: I want to show error if number is negative.**

A:

```csharp
if (number < 0)
{
    MessageBox.Show("Invalid number");
}
```

**Q49: I want to check two conditions in UI.**

A:

```csharp
if (checkBox1.Checked && score > 10)
{
    label1.Text = "OK";
}
```

**Q50: I want to disable UI when not logged in.**

A:

```csharp
button1.Enabled = false;
```

</details>

<details>
<summary><h3>Random Numbers (WinForms)</h3></summary>

**Q51: I want to generate random number for label.**

A:

```csharp
Random rand = new Random();
label1.Text = rand.Next(1, 11).ToString();
```

**Q52: I want to simulate a dice roll.**

A:

```csharp
Random rand = new Random();
int roll = rand.Next(1, 7);
label1.Text = roll.ToString();
```

**Q53: I want to randomly enable a button.**

A:

```csharp
Random rand = new Random();
button1.Enabled = rand.Next(2) == 0;
```

**Q54: I want to flip a coin in UI.**

A:

```csharp
Random rand = new Random();
label1.Text = rand.Next(2) == 0 ? "Heads" : "Tails";
```

**Q55: I want to randomly pick a name.**

A:

```csharp
string[] names = { "Alex", "Sam", "Jordan" };
Random rand = new Random();
label1.Text = names[rand.Next(names.Length)];
```

**Q56: I want to generate random damage value.**

A:

```csharp
Random rand = new Random();
int damage = rand.Next(5, 16);
```

**Q57: I want to randomize score gain.**

A:

```csharp
Random rand = new Random();
score += rand.Next(1, 6);
```

**Q58: I want to randomly change label text.**

A:

```csharp
string[] texts = { "Win", "Lose", "Try Again" };
Random rand = new Random();
label1.Text = texts[rand.Next(texts.Length)];
```

**Q59: I want to simulate random event trigger.**

A:

```csharp
Random rand = new Random();
if (rand.Next(100) < 30)
{
    MessageBox.Show("Event triggered!");
}
```

**Q60: I want to generate random background logic trigger.**

A:

```csharp
Random rand = new Random();
panel1.Enabled = rand.Next(2) == 1;
```

</details>
</details>

<details>
<summary><h2>Flowcharts + Key</h2></summary>

<details>
<summary><h3>Flowchart Shape Key</h3></summary>

| Text notation | Actual shape | Meaning |
| --- | --- | --- |
| `([ START / END ])` | **Oval / Terminator** | Start or end |
| `[ Process ]` | **Rectangle** | Calculation, assignment, conversion, setup |
| `[/ Input / Output /]` | **Parallelogram** | Read from or write to the UI |
| `{ Condition? }` | **Diamond** | Decision / branching |
| `↓` | **Arrow** | Direction of execution |

</details>

<details>
<summary><h3>Project 1: Simple Calculator — WinForms</h3></summary>

#### Text-based flowchart

```
         ([ START ])
              |
              ↓
     [ Button Add clicked ]
              |
              ↓
[/ Read TextBox1.Text /]
              |
              ↓
[ Convert TextBox1 input
      to integer ]
              |
              ↓
[/ Read TextBox2.Text /]
              |
              ↓
[ Convert TextBox2 input
      to integer ]
              |
              ↓
[ Calculate:
  result = num1 + num2 ]
              |
              ↓
[/ Convert result to text /]
              |
              ↓
[/ Display result
   in labelResult /]
              |
              ↓
          ([ END ])
```

#### Shape breakdown

- Button clicked → **Process**
- Read `textBox1` → **Input/Output**
- `int.Parse()` → **Process**
- Read `textBox2` → **Input/Output**
- `int.Parse()` → **Process**
- Addition → **Process**
- `ToString()` → **Process**
- Update `labelResult` → **Input/Output**

#### Important WinForms concept

The program isn't continuously running this sequence. The **button click event triggers the flow**:

```
User clicks button
      ↓
buttonAdd_Click()
      ↓
Program logic
      ↓
UI updates
```

</details>

<details>
<summary><h3>Project 2: Name Greeting App</h3></summary>

#### Text-based flowchart

```
         ([ START ])
              |
              ↓
    [ Button Greet clicked ]
              |
              ↓
[/ Read name from
   textBoxName /]
              |
              ↓
[ Create greeting message:
  "Hello, " + name + "!" ]
              |
              ↓
[/ Store greeting
   in message /]
              |
              ↓
[/ Display message
   in labelGreeting /]
              |
              ↓
          ([ END ])
```

#### Shape breakdown

- Button clicked → **Process**
- Read textbox → **Input/Output**
- Create message → **Process**
- Store message → **Process**
- Display message → **Input/Output**

#### Core flow

```
TextBox
  ↓
name
  ↓
"Hello, " + name + "!"
  ↓
Label
```

This is essentially:

**UI Input → Processing → UI Output**

</details>

<details>
<summary><h3>Project 3: Number Guessing Game</h3></summary>

#### Text-based flowchart

```
         ([ START ])
              |
              ↓
    [ Button Guess clicked ]
              |
              ↓
    [ Generate random
      number 1–10 ]
              |
              ↓
[/ Read guess from
   textBoxGuess /]
              |
              ↓
[ Convert guess
      to integer ]
              |
              ↓
      { guess == secretNumber? }
            /             \
          YES              NO
           |                |
           ↓                ↓
[/ Set labelResult to   [/ Set labelResult to
    "Correct!" /]          "Wrong! It was
                            " + secretNumber /]
           |                |
           └────────┬───────┘
                    ↓
                ([ END ])
```

#### Shape breakdown

- Button clicked → **Process**
- Generate random number → **Process**
- Read guess → **Input/Output**
- Convert guess → **Process**
- Compare values → **Decision**
- Display `"Correct!"` → **Input/Output**
- Display wrong result → **Input/Output**
- End → **Terminator**

#### Core logic

```
              guess == secretNumber?
                 /          \
               YES           NO
                ↓             ↓
             Correct         Wrong
```

</details>

<details>
<summary><h3>Project 4: Simple Grade Checker</h3></summary>

This is the most complex of the five because it introduces an **`if → else if → else` decision chain**.

#### Text-based flowchart

```
         ([ START ])
              |
              ↓
    [ Button Check clicked ]
              |
              ↓
[/ Read score from
   textBoxScore /]
              |
              ↓
[ Convert score
      to integer ]
              |
              ↓
      { score >= 90? }
         /         \
       YES          NO
        |            |
        ↓            ↓
[/ Display A /]   { score >= 80? }
                       /       \
                     YES        NO
                      |          |
                      ↓          ↓
               [/ Display B /] { score >= 70? }
                                  /       \
                                YES        NO
                                 |          |
                                 ↓          ↓
                          [/ Display C /] { score >= 60? }
                                             /       \
                                           YES        NO
                                            |          |
                                            ↓          ↓
                                     [/ Display D /] [/ Display F /]
                                            |          |
                                            └────┬─────┘
                                                 ↓
                                             ([ END ])
```

#### Shape breakdown

- Button clicked → **Process**
- Read score → **Input/Output**
- Convert score → **Process**
- `score >= 90` → **Decision**
- `score >= 80` → **Decision**
- `score >= 70` → **Decision**
- `score >= 60` → **Decision**
- Display grade → **Input/Output**
- End → **Terminator**

#### Logic view

```
             score >= 90?
             /         \
           YES          NO
            ↓            ↓
            A        score >= 80?
                      /         \
                    YES          NO
                     ↓            ↓
                     B       score >= 70?
                              /        \
                            YES         NO
                             ↓           ↓
                             C      score >= 60?
                                     /       \
                                   YES        NO
                                    ↓          ↓
                                    D          F
```

This is a good example of how **multiple diamonds can form one logical decision tree**.

</details>

<details>
<summary><h3>Project 5: Dice Roller App</h3></summary>

#### Text-based flowchart

```
         ([ START ])
              |
              ↓
     [ Button Roll clicked ]
              |
              ↓
   [ Generate random number
         between 1–6 ]
              |
              ↓
      [ Store result
         in roll ]
              |
              ↓
[/ Create display text:
   "You rolled: " + roll /]
              |
              ↓
[/ Display text
   in labelRoll /]
              |
              ↓
          ([ END ])
```

#### Shape breakdown

- Button clicked → **Process**
- Generate random number → **Process**
- Store roll → **Process**
- Create display text → **Process**
- Update label → **Input/Output**
- End → **Terminator**

#### Core flow

```
Button
  ↓
Random Number
  ↓
roll
  ↓
"You rolled: " + roll
  ↓
Label
```

</details>

<details>
<summary><h3>All 5 WinForms Flows Together</h3></summary>

You can see a nice progression here:

```
PROJECT 1
Calculator
│
├── UI Input
├── Conversion
├── Calculation
└── UI Output
       ↓
PROJECT 2
Greeting
│
├── UI Input
├── String processing
└── UI Output
       ↓
PROJECT 3
Guessing Game
│
├── Random generation
├── UI Input
├── Conversion
├── Decision
└── UI Output
       ↓
PROJECT 4
Grade Checker
│
├── UI Input
├── Conversion
├── Multiple decisions
└── UI Output
       ↓
PROJECT 5
Dice Roller
│
├── Button event
├── Random generation
├── String construction
└── UI Output
```

#### The bigger WinForms pattern

All five projects are basically teaching this architecture:

```
            USER
             │
             ↓
      ┌──────────────┐
      │ UI CONTROL   │
      │ Button/Input │
      └──────┬───────┘
             │
             ↓
      ┌──────────────┐
      │ EVENT HANDLER│
      │ button_Click │
      └──────┬───────┘
             │
             ↓
      ┌──────────────┐
      │ PROGRAM      │
      │ LOGIC        │
      └──────┬───────┘
             │
             ↓
      ┌──────────────┐
      │ UI OUTPUT    │
      │ Label/TextBox│
      └──────────────┘
```

That's probably the **most important flowchart to put at the top of your WinForms notes**, because it gives you the big picture before getting into individual projects.

</details>
</details>

<details>
<summary><h2>Sample Projects</h2></summary>

<details>
<summary><h3>Project 1: Simple Calculator (WinForms)</h3></summary>

#### What it does

Takes two numbers from textboxes and shows sum.

#### Steps

1. Get input from TextBox1
2. Get input from TextBox2
3. Convert to numbers
4. Add numbers
5. Display result in Label

```csharp
using System;
using System.Windows.Forms;

public partial class Form1 : Form
{
    public Form1()
    {
        InitializeComponent();
    }

    private void buttonAdd_Click(object sender, EventArgs e)
    {
        // Step 1: Get input from first textbox
        int num1 = int.Parse(textBox1.Text);

        // Step 2: Get input from second textbox
        int num2 = int.Parse(textBox2.Text);

        // Step 3: Add numbers together
        int result = num1 + num2;

        // Step 4: Show result in label
        labelResult.Text = result.ToString();
    }
}
```

</details>

<details>
<summary><h3>Project 2: Name Greeting App</h3></summary>

#### What it does

User enters name → app greets them.

#### Steps

1. Get name input
2. Create greeting message
3. Display message in label

```csharp
using System;
using System.Windows.Forms;

public partial class Form1 : Form
{
    public Form1()
    {
        InitializeComponent();
    }

    private void buttonGreet_Click(object sender, EventArgs e)
    {
        // Step 1: Get user name from textbox
        string name = textBoxName.Text;

        // Step 2: Create greeting message
        string message = "Hello, " + name + "!";

        // Step 3: Display message in label
        labelGreeting.Text = message;
    }
}
```

</details>

<details>
<summary><h3>Project 3: Number Guessing Game</h3></summary>

#### What it does

User guesses a random number from 1–10.

#### Steps

1. Generate random number
2. Get user guess
3. Compare values
4. Show result

```csharp
using System;
using System.Windows.Forms;

public partial class Form1 : Form
{
    Random rand = new Random();

    public Form1()
    {
        InitializeComponent();
    }

    private void buttonGuess_Click(object sender, EventArgs e)
    {
        // Step 1: Generate random number
        int secretNumber = rand.Next(1, 11);

        // Step 2: Get user guess
        int guess = int.Parse(textBoxGuess.Text);

        // Step 3: Compare numbers
        if (guess == secretNumber)
        {
            labelResult.Text = "Correct!";
        }
        else
        {
            labelResult.Text = "Wrong! It was " + secretNumber;
        }
    }
}
```

</details>

<details>
<summary><h3>Project 4: Simple Grade Checker</h3></summary>

#### What it does

Converts score into letter grade.

#### Steps

1. Get score input
2. Convert to number
3. Check range
4. Display grade

```csharp
using System;
using System.Windows.Forms;

public partial class Form1 : Form
{
    public Form1()
    {
        InitializeComponent();
    }

    private void buttonCheck_Click(object sender, EventArgs e)
    {
        // Step 1: Get score input
        int score = int.Parse(textBoxScore.Text);

        // Step 2: Determine grade
        if (score >= 90)
        {
            labelGrade.Text = "A";
        }
        else if (score >= 80)
        {
            labelGrade.Text = "B";
        }
        else if (score >= 70)
        {
            labelGrade.Text = "C";
        }
        else if (score >= 60)
        {
            labelGrade.Text = "D";
        }
        else
        {
            labelGrade.Text = "F";
        }
    }
}
```

</details>

<details>
<summary><h3>Project 5: Dice Roller App</h3></summary>

#### What it does

Rolls a dice and shows result in UI.

#### Steps

1. Create random generator
2. Generate number 1–6
3. Display result

```csharp
using System;
using System.Windows.Forms;

public partial class Form1 : Form
{
    Random rand = new Random();

    public Form1()
    {
        InitializeComponent();
    }

    private void buttonRoll_Click(object sender, EventArgs e)
    {
        // Step 1: Generate dice roll (1–6)
        int roll = rand.Next(1, 7);

        // Step 2: Display result
        labelRoll.Text = "You rolled: " + roll;
    }
}
```

</details>
</details>