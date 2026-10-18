<details>
<summary><h1>Coding Basics/White Belt/Javascript + GUI (HTML/CSS)</h1></summary>

💡 Tip: Click the arrows next to each heading to expand or collapse the content underneath.

<details>
<summary><h2>Key Concepts</h2></summary>

<details>
<summary><h3>Variables & Constants</h3></summary>

Q1: What is a variable?

A: A variable is a named box that stores information your web page can use or change.

Q2: When should I use a variable?

A: Use a variable whenever a value might change, like a score, username, or counter.

Q3: What is a constant?

A: A constant is a value that should never change after it is created.

Q4: When should I use a constant instead of a variable?

A: Use a constant for fixed values like tax rates or your application's name.

Q5: Why should I use meaningful variable names?

A: Good names make your code easier to read and maintain.

Q6: How do I create a variable?

A:

```jsx

let score = 0;

```

Q7: How do I create a constant?

A:

```jsx

const APP_NAME = "My Website";

```

Q8: Can I change a variable later?

A: Yes.

```jsx

let score = 10;

score = 20;

```

Q9: Can I change a constant later?

A: No. Constants cannot be reassigned.

Q10: Why are variables important in web pages?

A: They let your page remember information while the user interacts with it.

</details>
<details>
<summary><h3>Data Types</h3></summary>

Q11: What is a data type?

A: A data type tells JavaScript what kind of information is stored.

Q12: What is a number?

A: A number stores whole numbers and decimals.

```jsx

let age = 25;

```

Q13: What is a string?

A: A string stores text.

```jsx

let name = "Alice";

```

Q14: What is a boolean?

A: A boolean stores either true or false.

```jsx

let isLoggedIn = true;

```

Q15: What is null?

A: Null means a variable intentionally has no value.

Q16: What is undefined?

A: Undefined means a variable hasn't been given a value yet.

Q17: When should I use a string instead of a number?

A: Use strings for text and numbers for calculations.

Q18: Why should I use the correct data type?

A: It helps prevent bugs and makes your code easier to understand.

Q19: Can JavaScript change a variable's data type?

A: Yes, but it's usually better to keep variables consistent.

Q20: How do I choose the right data type?

A: Decide whether you're storing text, numbers, or true/false values.

</details>
<details>
<summary><h3>Input / Output (HTML/CSS + JavaScript)</h3></summary>

Q21: What is input?

A: Input is information the user enters into your webpage.

Q22: How do I get text from a textbox?

A:

```jsx

let name = document.getElementById("txtName").value;

```

Q23: What is output?

A: Output is information displayed on the webpage.

Q24: How do I display text inside a label or paragraph?

A:

```jsx

document.getElementById("output").textContent = "Hello!";

```

Q25: How do I display a popup message?

A:

```jsx

alert("Hello!");

```

Q26: Why use HTML elements instead of console.log()?

A: Because website users see the webpage, not the browser console.

Q27: How do I change button text?

A:

```jsx

document.getElementById("btnSave").textContent = "Saved!";

```

Q28: How do I clear a textbox?

A:

```jsx

document.getElementById("txtName").value = "";

```

Q29: Why do I use document.getElementById()?

A: It finds an HTML element so JavaScript can use it.

Q30: What is the .value property?

A: It gets or sets the text inside input controls.

</details>
<details>
<summary><h3>Basic Math Operations</h3></summary>

Q31: How do I add two numbers?

A:

```jsx

let total = a + b;

```

Q32: How do I subtract two numbers?

A:

```jsx

let result = a - b;

```

Q33: How do I multiply two numbers?

A:

```jsx

let area = width * height;

```

Q34: How do I divide two numbers?

A:

```jsx

let answer = total / count;

```

Q35: What does the % operator do?

A: It gives the remainder after division.

Q36: How do I increase a counter by 1?

A:

```jsx

count++;

```

Q37: How do I decrease a counter by 1?

A:

```jsx

count--;

```

Q38: Why store math results in variables?

A: So you can display or reuse them later.

Q39: How do I calculate the average of two numbers?

A:

```jsx

let average = (a + b) / 2;

```

Q40: Why is math useful in websites?

A: Websites often calculate prices, scores, totals, and statistics.

</details>
<details>
<summary><h3>Conditionals (if / else)</h3></summary>

Q41: What is an if statement?

A: It lets your webpage make decisions.

Q42: When should I use an if statement?

A: Whenever something should only happen if a condition is true.

Q43: What is an else statement?

A: It runs when the if condition is false.

Q44: How do I write an if statement?

A:

```jsx

if (age >= 18)

{

    alert("Adult");

}

```

Q45: How do I use if and else together?

A:

```jsx

if (score >= 60)

{

    alert("Pass");

}

else

{

    alert("Fail");

}

```

Q46: What is a condition?

A: A condition is a question that is either true or false.

Q47: What comparison operators are commonly used?

A:

```

\==

\===

!=

<

>

<=

>=

```

Q48: Why are conditionals important?

A: They let your webpage react differently based on user input.

Q49: How do I check multiple conditions?

A:

```jsx

if (age >= 18 && hasID)

{

    alert("Access Granted");

}

```

Q50: What is the easiest way to think about an if statement?

A: Think of it as asking a yes-or-no question before doing something.

</details>
<details>
<summary><h3>Random Numbers</h3></summary>

Q51: What is a random number?

A: A number chosen unpredictably.

Q52: When should I use random numbers?

A: For games, quizzes, random colors, or random choices.

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

Q55: Why do I use Math.floor()?

A: It removes the decimal part to make a whole number.

Q56: What does Math.random() return?

A: A decimal from 0 up to (but not including) 1.

Q57: How do I simulate rolling a die?

A:

```jsx

let roll = Math.floor(Math.random() * 6) + 1;

```

Q58: How do I randomly choose true or false?

A:

```jsx

let result = Math.random() < 0.5;

```

Q59: How do I randomly choose an item from an array?

A:

```jsx

let names = ["Alex", "Sam", "Jordan"];

let pick = names[Math.floor(Math.random() * names.length)];

```

Q60: Why are random numbers useful on websites?

A: They make web pages more interactive, dynamic, and fun.

</details>
</details>
<details>
<summary><h2>Code Syntax</h2></summary>

<details>
<summary><h3>Variables & Constants</h3></summary>

Q1: I want to store the user's name from a textbox.

A:

```jsx

let name = document.getElementById("txtName").value;

```

Q2: I want to store a score that changes while the app runs.

A:

```jsx

let score = 0;

```

Q3: I want to store a fixed app title.

A:

```jsx

const APP_NAME = "My App";

```

Q4: I want to store whether a checkbox is checked.

A:

```jsx

let isChecked = document.getElementById("chkAgree").checked;

```

Q5: I want to increase a score by 10.

A:

```jsx

score += 10;

```

Q6: I want to reset a score to zero.

A:

```jsx

score = 0;

```

Q7: I want to store a decimal price.

A:

```jsx

let price = 19.99;

```

Q8: I want to update a username variable.

A:

```jsx

username = "Alex";

```

Q9: I want to store a player's health.

A:

```jsx

let health = 100;

```

Q10: I want to store whether dark mode is enabled.

A:

```jsx

let darkMode = true;

```

</details>
<details>
<summary><h3>Data Types</h3></summary>

Q11: I want to convert textbox input into a number.

A:

```jsx

let age = Number(document.getElementById("txtAge").value);

```

Q12: I want to store text entered by the user.

A:

```jsx

let message = document.getElementById("txtMessage").value;

```

Q13: I want to store a true/false value.

A:

```jsx

let loggedIn = false;

```

Q14: I want to store a decimal number.

A:

```jsx

let temperature = 72.5;

```

Q15: I want to convert text into a decimal number.

A:

```jsx

let price = parseFloat(document.getElementById("txtPrice").value);

```

Q16: I want to store a large number.

A:

```jsx

let population = 8000000;

```

Q17: I want to store multiple words.

A:

```jsx

let title = "Hello World";

```

Q18: I want to store whether a button is enabled.

A:

```jsx

let enabled = true;

```

Q19: I want to convert a string into an integer.

A:

```jsx

let quantity = parseInt(document.getElementById("txtQuantity").value);

```

Q20: I want to store a product name.

A:

```jsx

let product = "Laptop";

```

</details>
<details>
<summary><h3>Input / Output (HTML/CSS)</h3></summary>

Q21: I want to display text inside a paragraph.

A:

```jsx

document.getElementById("output").textContent = "Hello!";

```

Q22: I want to read text from a textbox.

A:

```jsx

let input = document.getElementById("txtInput").value;

```

Q23: I want to display a popup message.

A:

```jsx

alert("Welcome!");

```

Q24: I want to clear a textbox.

A:

```jsx

document.getElementById("txtInput").value = "";

```

Q25: I want to change the text of a button.

A:

```jsx

document.getElementById("btnSave").textContent = "Saved";

```

Q26: I want to display the user's name.

A:

```jsx

document.getElementById("lblName").textContent = name;

```

Q27: I want to change a heading.

A:

```jsx

document.getElementById("title").textContent = "Dashboard";

```

Q28: I want to display a calculation result.

A:

```jsx

document.getElementById("result").textContent = total;

```

Q29: I want to display multiple lines.

A:

```jsx

document.getElementById("output").innerHTML = "Line 1<br>Line 2";

```

Q30: I want to clear displayed text.

A:

```jsx

document.getElementById("output").textContent = "";

```

</details>
<details>
<summary><h3>Basic Math Operations</h3></summary>

Q31: I want to add two textbox numbers.

A:

```jsx

let total =

    Number(document.getElementById("txtA").value) +

    Number(document.getElementById("txtB").value);

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

Q36: I want to increase a counter.

A:

```jsx

count++;

```

Q37: I want to decrease a counter.

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

Q41: I want to check if a textbox is empty.

A:

```jsx

if (document.getElementById("txtName").value === "")

{

    alert("Please enter a name.");

}

```

Q42: I want to check if someone is 18 or older.

A:

```jsx

if (age >= 18)

{

    alert("Access Granted");

}

```

Q43: I want to show pass or fail.

A:

```jsx

if (score >= 60)

{

    alert("Pass");

}

else

{

    alert("Fail");

}

```

Q44: I want to check if two values are equal.

A:

```jsx

if (a === b)

{

    alert("Equal");

}

```

Q45: I want to check if both conditions are true.

A:

```jsx

if (loggedIn && isAdmin)

{

    alert("Welcome Admin");

}

```

Q46: I want to check if either condition is true.

A:

```jsx

if (isAdmin || isModerator)

{

    alert("Access Granted");

}

```

Q47: I want to check if a number is not zero.

A:

```jsx

if (number !== 0)

{

    alert("Valid");

}

```

Q48: I want to display a letter grade.

A:

```jsx

if (score >= 90)

{

    grade = "A";

}

else if (score >= 80)

{

    grade = "B";

}

else

{

    grade = "C";

}

```

Q49: I want to check if a checkbox is checked.

A:

```jsx

if (document.getElementById("chkAgree").checked)

{

    alert("Thank you!");

}

```

Q50: I want to display a message only when the user is logged in.

A:

```jsx

if (loggedIn)

{

    alert("Welcome Back!");

}

```

</details>
<details>
<summary><h3>Random Numbers</h3></summary>

Q51: I want to generate a random number from 1 to 10.

A:

```jsx

let number = Math.floor(Math.random() * 10) + 1;

```

Q52: I want to simulate rolling a die.

A:

```jsx

let roll = Math.floor(Math.random() * 6) + 1;

```

Q53: I want to randomly choose true or false.

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

Q57: I want to randomly increase score by 1–5.

A:

```jsx

score += Math.floor(Math.random() * 5) + 1;

```

Q58: I want to randomly choose a color.

A:

```jsx

let colors = ["red", "blue", "green"];

let color = colors[Math.floor(Math.random() * colors.length)];

```

Q59: I want to randomly choose a player's name.

A:

```jsx

let players = ["Alex", "Sam", "Jordan"];

let player = players[Math.floor(Math.random() * players.length)];

```

Q60: I want to randomly decide whether an attack hits.

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

| `([ START / END ])` | ****Oval / Terminator**** | Start or end |

| `[ Process ]` | ****Rectangle**** | Calculation, assignment, transformation |

| `[/ Input / Output /]` | ****Parallelogram**** | User input or webpage output |

| `{ Condition? }` | ****Diamond**** | Decision / branching |

| `↓` | ****Arrow**** | Direction of execution |

</details>
<details>
<summary><h3>Project 1: Simple Web Calculator</h3></summary>

<details>
<summary><h4>Text-based flowchart</h4></summary>

```

             ([ START ])

                  |

                  ↓

       [ User clicks "Add" button ]

                  |

                  ↓

       [ Call addNumbers() ]

                  |

                  ↓

       [/ Get value from num1 /]

                  |

                  ↓

       [ Convert value to Number ]

                  |

                  ↓

       [/ Get value from num2 /]

                  |

                  ↓

       [ Convert value to Number ]

                  |

                  ↓

       [ Calculate:

         sum = a + b ]

                  |

                  ↓

       [/ Display sum in

          result element /]

                  |

                  ↓

              ([ END ])

```

</details>
<details>
<summary><h4>Shape breakdown</h4></summary>

- User clicks button → ****Input/Output****

- Call `addNumbers()` → ****Process****

- Get input value → ****Input/Output****

- `Number()` conversion → ****Process****

- Addition → ****Process****

- Update HTML element → ****Input/Output****

- End → ****Terminator****

</details>
<details>
<summary><h4>Core architecture</h4></summary>

```

HTML Input

    ↓

Button Click

    ↓

JavaScript Function

    ↓

Get Values

    ↓

Process

    ↓

DOM Update

    ↓

HTML Output

```

</details>
</details>
<details>
<summary><h3>Project 2: Name Greeting App</h3></summary>

<details>
<summary><h4>Text-based flowchart</h4></summary>

```

             ([ START ])

                  |

                  ↓

       [ User clicks "Greet" ]

                  |

                  ↓

          [ Call greet() ]

                  |

                  ↓

       [/ Get nameInput value /]

                  |

                  ↓

       [ Create message:

         "Hello, " + name + "!" ]

                  |

                  ↓

       [/ Display message

          in output element /]

                  |

                  ↓

              ([ END ])

```

</details>
<details>
<summary><h4>Shape breakdown</h4></summary>

- Button click → ****Input/Output****

- Call function → ****Process****

- Get name → ****Input/Output****

- Build greeting → ****Process****

- Update `<h2>` → ****Input/Output****

- End → ****Terminator****

</details>
<details>
<summary><h4>Core logic</h4></summary>

```

User

 ↓

Input

 ↓

JavaScript

 ↓

Create String

 ↓

DOM

 ↓

Webpage

```

</details>
</details>
<details>
<summary><h3>Project 3: Number Guessing Game</h3></summary>

<details>
<summary><h4>Text-based flowchart</h4></summary>

```

             ([ START ])

                  |

                  ↓

       [ User clicks "Guess" ]

                  |

                  ↓

       [ Call checkGuess() ]

                  |

                  ↓

       [ Generate random

         number from 1–10 ]

                  |

                  ↓

       [/ Get guessInput value /]

                  |

                  ↓

       [ Convert guess to Number ]

                  |

                  ↓

          { guess === secret? }

             /            \\

           YES             NO

            |               |

            ↓               ↓

 [/ Set result to       [/ Set result to

      "Correct!" /]       "Wrong! It was"

                          + secret /]

            |               |

            └───────┬───────┘

                    ↓

        [/ Update result element /]

                    |

                    ↓

                ([ END ])

```

</details>
<details>
<summary><h4>Shape breakdown</h4></summary>

- Button click → ****Input/Output****

- Call function → ****Process****

- Generate random number → ****Process****

- Get guess → ****Input/Output****

- Convert guess → ****Process****

- Compare values → ****Decision****

- Set result → ****Input/Output****

- End → ****Terminator****

</details>
<details>
<summary><h4>Core decision</h4></summary>

```

              { guess === secret? }

                  /          \\

                YES           NO

                 ↓             ↓

             Correct         Wrong

```

This is the first project in the group that introduces a ****branch in program execution****.

</details>
</details>
<details>
<summary><h3>Project 4: Simple Grade Checker</h3></summary>

This one demonstrates a ****multi-branch decision tree****.

<details>
<summary><h4>Text-based flowchart</h4></summary>

```

             ([ START ])

                  |

                  ↓

       [ User clicks "Check Grade" ]

                  |

                  ↓

          [ Call checkGrade() ]

                  |

                  ↓

       [/ Get scoreInput value /]

                  |

                  ↓

       [ Convert score to Number ]

                  |

                  ↓

           { score >= 90? }

             /          \\

           YES           NO

            |             |

            ↓             ↓

        [ grade = "A" ] { score >= 80? }

                           /         \\

                         YES          NO

                          |            |

                          ↓            ↓

                    [ grade = "B" ] { score >= 70? }

                                      /        \\

                                    YES         NO

                                     |           |

                                     ↓           ↓

                               [ grade = "C" ] { score >= 60? }

                                                   /       \\

                                                 YES        NO

                                                  |          |

                                                  ↓          ↓

                                            [ grade = "D" ] [ grade = "F" ]

                                                  |          |

                                                  └────┬─────┘

                                                       ↓

                                           [/ Display grade

                                              in grade element /]

                                                       |

                                                       ↓

                                                   ([ END ])

```

</details>
<details>
<summary><h4>Shape breakdown</h4></summary>

- Button click → ****Input/Output****

- Call function → ****Process****

- Read score → ****Input/Output****

- Convert score → ****Process****

- `score >= 90` → ****Decision****

- `score >= 80` → ****Decision****

- `score >= 70` → ****Decision****

- `score >= 60` → ****Decision****

- Assign grade → ****Process****

- Display grade → ****Input/Output****

- End → ****Terminator****

</details>
<details>
<summary><h4>Logic view</h4></summary>

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

One useful distinction here:

****The diamonds determine the grade; the rectangle assigns it.****

```

{ score >= 90? }    ← Decision

        ↓

[ grade = "A" ]     ← Process

```

</details>
</details>
<details>
<summary><h3>Project 5: Random Color Changer</h3></summary>

<details>
<summary><h4>Text-based flowchart</h4></summary>

```

             ([ START ])

                  |

                  ↓

       [ User clicks "Change Color" ]

                  |

                  ↓

          [ Call changeColor() ]

                  |

                  ↓

       [ Generate random R value

             between 0–255 ]

                  |

                  ↓

       [ Generate random G value

             between 0–255 ]

                  |

                  ↓

       [ Generate random B value

             between 0–255 ]

                  |

                  ↓

       [ Build RGB color string:

         "rgb(" + r + "," + g + "," + b + ")" ]

                  |

                  ↓

       [ Set document.body

         backgroundColor = color ]

                  |

                  ↓

             ([ END ])

```

</details>
<details>
<summary><h4>Shape breakdown</h4></summary>

- Button click → ****Input/Output****

- Call function → ****Process****

- Generate `r` → ****Process****

- Generate `g` → ****Process****

- Generate `b` → ****Process****

- Build RGB string → ****Process****

- Change webpage background → ****Process****

- End → ****Terminator****

</details>
<details>
<summary><h4>Core architecture</h4></summary>

```

Button

  ↓

JavaScript Function

  ↓

Random R

  ↓

Random G

  ↓

Random B

  ↓

Build RGB String

  ↓

Modify DOM/CSS

  ↓

Background Changes

```

</details>
</details>
<details>
<summary><h3>All 5 projects — progression</h3></summary>

These five give you a pretty clean progression in ****web programming logic****:

```

PROJECT 1

Simple Calculator

        ↓

DOM INPUT

        ↓

JavaScript PROCESSING

        ↓

DOM OUTPUT

        ↓

PROJECT 2

Name Greeting

        ↓

String Processing

        ↓

DOM OUTPUT

        ↓

PROJECT 3

Number Guessing

        ↓

Random Data

        ↓

Decision

        ↓

Different Outputs

        ↓

PROJECT 4

Grade Checker

        ↓

Multiple Decisions

        ↓

Decision Tree

        ↓

PROJECT 5

Random Color Changer

        ↓

Random Data

        ↓

String Construction

        ↓

DOM/CSS Manipulation

```

<details>
<summary><h4>The common web-programming pattern</h4></summary>

You can use this as the ****master flowchart**** for your notes:

```

              ([ START ])

                   |

                   ↓

          [/ USER INTERACTION /]

                   |

                   ↓

           [ JavaScript Event ]

                   |

                   ↓

          [ JavaScript Function ]

                   |

                   ↓

          [/ GET HTML DATA /]

                   |

                   ↓

             [ PROCESS DATA ]

                   |

                   ↓

              { DECISION? }

               /        \\

             YES         NO

              |           |

              ↓           ↓

         [ Process ]  [ Process ]

              |           |

              └─────┬─────┘

                    ↓

             [ UPDATE DOM ]

                    |

                    ↓

          [/ DISPLAY ON PAGE /]

                    |

                    ↓

                ([ END ])

```

The big idea you're teaching with these projects is:

****HTML provides the interface → JavaScript responds to events → JavaScript processes data → JavaScript manipulates the DOM → the webpage changes.****

</details>
</details>
</details>
<details>
<summary><h2>Sample Projects</h2></summary>

<details>
<summary><h3>Project 1: Simple Web Calculator</h3></summary>

<details>
<summary><h4>What it does</h4></summary>

Takes two numbers from input boxes and displays the sum on a webpage.

</details>
<details>
<summary><h4>Steps</h4></summary>

1\. Get number from first input

2\. Get number from second input

3\. Convert both to numbers

4\. Add them together

5\. Display result in HTML

```html

<!DOCTYPE html>

<html>

<head>

    <title>Calculator</title>

</head>

<body>

<input id="num1" placeholder="First number">

<input id="num2" placeholder="Second number">

<button onclick="addNumbers()">Add</button>

<p id="result"></p>

<script>

// Step 1: Create function triggered by button

function addNumbers() {

    // Step 2: Get first input value

    let a = Number(document.getElementById("num1").value);

    // Step 3: Get second input value

    let b = Number(document.getElementById("num2").value);

    // Step 4: Add numbers

    let sum = a + b;

    // Step 5: Display result on page

    document.getElementById("result").textContent = sum;

}

</script>

</body>

</html>

```

</details>
</details>
<details>
<summary><h3>Project 2: Name Greeting App</h3></summary>

<details>
<summary><h4>What it does</h4></summary>

User enters name → webpage greets them.

</details>
<details>
<summary><h4>Steps</h4></summary>

1\. Get name from input

2\. Create greeting message

3\. Show message on page

```html

<!DOCTYPE html>

<html>

<body>

<input id="nameInput" placeholder="Enter name">

<button onclick="greet()">Greet</button>

<h2 id="output"></h2>

<script>

function greet() {

    // Step 1: Get name from input

    let name = document.getElementById("nameInput").value;

    // Step 2: Create message

    let message = "Hello, " + name + "!";

    // Step 3: Display message

    document.getElementById("output").textContent = message;

}

</script>

</body>

</html>

```

</details>
</details>
<details>
<summary><h3>Project 3: Number Guessing Game</h3></summary>

<details>
<summary><h4>What it does</h4></summary>

User guesses a random number between 1–10.

</details>
<details>
<summary><h4>Steps</h4></summary>

1\. Generate random number

2\. Get user guess

3\. Compare values

4\. Show result

```html

<!DOCTYPE html>

<html>

<body>

<input id="guessInput" placeholder="Guess 1-10">

<button onclick="checkGuess()">Guess</button>

<p id="result"></p>

<script>

function checkGuess() {

    // Step 1: Generate random number

    let secret = Math.floor(Math.random() * 10) + 1;

    // Step 2: Get user guess

    let guess = Number(document.getElementById("guessInput").value);

    // Step 3: Compare values

    if (guess === secret) {

        // Step 4A: Correct guess

        document.getElementById("result").textContent = "Correct!";

    } else {

        // Step 4B: Wrong guess

        document.getElementById("result").textContent =

            "Wrong! It was " + secret;

    }

}

</script>

</body>

</html>

```

</details>
</details>
<details>
<summary><h3>Project 4: Simple Grade Checker</h3></summary>

<details>
<summary><h4>What it does</h4></summary>

Converts a score into a letter grade.

</details>
<details>
<summary><h4>Steps</h4></summary>

1\. Get score input

2\. Convert to number

3\. Check grade range

4\. Display grade

```html

<!DOCTYPE html>

<html>

<body>

<input id="scoreInput" placeholder="Enter score">

<button onclick="checkGrade()">Check Grade</button>

<p id="grade"></p>

<script>

function checkGrade() {

    // Step 1: Get score input

    let score = Number(document.getElementById("scoreInput").value);

    // Step 2: Determine grade

    let grade;

    if (score >= 90) {

        grade = "A";

    }

    else if (score >= 80) {

        grade = "B";

    }

    else if (score >= 70) {

        grade = "C";

    }

    else if (score >= 60) {

        grade = "D";

    }

    else {

        grade = "F";

    }

    // Step 3: Display grade

    document.getElementById("grade").textContent = grade;

}

</script>

</body>

</html>

```

</details>
</details>
<details>
<summary><h3>Project 5: Random Color Changer</h3></summary>

<details>
<summary><h4>What it does</h4></summary>

Click a button → page background changes color randomly.

</details>
<details>
<summary><h4>Steps</h4></summary>

1\. Create random RGB values

2\. Build color string

3\. Apply to page background

```html

<!DOCTYPE html>

<html>

<body>

<button onclick="changeColor()">Change Color</button>

<script>

function changeColor() {

    // Step 1: Generate random RGB values

    let r = Math.floor(Math.random() * 256);

    let g = Math.floor(Math.random() * 256);

    let b = Math.floor(Math.random() * 256);

    // Step 2: Create RGB color string

    let color = "rgb(" + r + "," + g + "," + b + ")";

    // Step 3: Apply color to page background

    document.body.style.backgroundColor = color;

}

</script>

</body>

</html>

```
</details>
</details>
</details>
</details>
