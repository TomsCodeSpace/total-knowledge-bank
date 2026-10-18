<details>
<summary><h1>Coding Basics/White Belt/Kotlin + GUI (XML)</h1></summary>

💡 Tip: Click the arrows next to each heading to expand or collapse the content underneath.

<details>
<summary><h2>Key Concepts</h2></summary>

<details>
<summary><h3>Variables and Constants</h3></summary>

### 1. What is a variable?

A variable is a container that stores information that can change while the program runs.

### 2. When should I use a variable?

Use a variable whenever you expect the value to change later.

### 3. Why should I use a variable?

Variables let your app remember information like scores, names, or health.

### 4. What is a constant?

A constant stores information that should never change after it is created.

### 5. What does `var` mean?

`var` creates a variable that can change.

### 6. What does `val` mean?

`val` creates a constant that cannot change.

</details>

<details>
<summary><h3>Data Types</h3></summary>

### 11. What is a data type?

A data type tells Kotlin what kind of information is being stored.

### 12. What is an Int?

An Int stores whole numbers like 5, 10, or 200.

### 13. What is a Double?

A Double stores decimal numbers.

### 14. What is a String?

A String stores text.

### 15. What is a Boolean?

A Boolean stores only two values: `true` and `false`.

</details>

<details>
<summary><h3>Input</h3></summary>

### 21. What is input?

Input is information the user gives your app.

### 22. What is an EditText?

An EditText is a textbox where users type information.

### 23. Why do I use `.text.toString()`?

Because EditText stores editable text, and you usually need a normal String.

### 24. What does `.toInt()` do?

It converts text into an integer.

### 25. What does `.toDouble()` do?

It converts text into a decimal number.

</details>

<details>
<summary><h3>Output</h3></summary>

### 31. What is output?

Output is information your app displays to the user.

### 32. What is a TextView?

A TextView displays text on the screen.

### 33. What is a Toast?

A Toast is a small popup message.

### 34. What does `.text =` do?

It changes what the TextView displays.

</details>

<details>
<summary><h3>Basic Math</h3></summary>

### 41. Why do programs perform math?

To calculate answers automatically.

### 42. What does `+` do?

Adds numbers.

### 43. What does `-` do?

Subtracts numbers.

### 44. What does `*` do?

Multiplies numbers.

### 45. What does `/` do?

Divides numbers.

### 46. What does `%` do?

Finds the remainder after division.

### 47. What does `++` do?

Adds one to a variable.

### 48. What does `--` do?

Subtracts one from a variable.

</details>

<details>
<summary><h3>Conditionals</h3></summary>

### 51. What is an if statement?

It lets your program make decisions.

### 52. What is an else statement?

It runs if the if statement is false.

### 53. What does `==` mean?

Checks if two values are equal.

### 54. What does `>` mean?

Checks if one value is greater than another.

### 55. What does `<` mean?

Checks if one value is less than another.

</details>

<details>
<summary><h3>Random Numbers</h3></summary>

### 59. What are random numbers?

Numbers chosen unpredictably by the computer.

### 60. When should I use random numbers?

Use them for dice rolls, card games, enemy behavior, loot drops, quizzes, and guessing games.

</details>

</details>

<details>
<summary><h2>Code Syntax</h2></summary>

<details>
<summary><h3>Variables and Constants</h3></summary>

**Q1: How do I create a variable that stores the player's score?**

```kotlin
var score = 0
```

**Q2: How do I create a constant that stores the app name?**

```kotlin
val appName = "My App"
```

**Q3: How do I store the user's name from an EditText?**

```kotlin
val name = editTextName.text.toString()
```

**Q4: How do I change a variable when a button is clicked?**

```kotlin
buttonIncrease.setOnClickListener {
    score++
}
```

**Q5: How do I display the value of a variable inside a TextView?**

```kotlin
textViewResult.text = score.toString()
```

</details>

<details>
<summary><h3>Data Types</h3></summary>

**Q11: How do I create an Int variable?**

```kotlin
var age: Int = 25
```

**Q12: How do I create a Double variable?**

```kotlin
var price: Double = 19.99
```

**Q13: How do I create a Boolean variable?**

```kotlin
var isOnline: Boolean = true
```

**Q14: How do I create a String variable?**

```kotlin
var city: String = "Kansas City"
```

**Q15: How do I convert text from an EditText into an Int?**

```kotlin
val number = editTextNumber.text.toString().toInt()
```

</details>

<details>
<summary><h3>Input / Output</h3></summary>

**Q21: How do I display "Hello World" inside a TextView?**

```kotlin
textViewResult.text = "Hello World"
```

**Q22: How do I display the text entered by the user?**

```kotlin
val input = editTextInput.text.toString()
textViewResult.text = input
```

**Q23: How do I clear an EditText?**

```kotlin
editTextInput.setText("")
```

**Q24: How do I display a Toast message?**

```kotlin
Toast.makeText(this, "Saved!", Toast.LENGTH_SHORT).show()
```

</details>

<details>
<summary><h3>Basic Math Operations</h3></summary>

**Q31: How do I add two numbers entered by the user?**

```kotlin
val result = num1 + num2
textViewResult.text = result.toString()
```

**Q32: How do I subtract two numbers?**

```kotlin
val result = num1 - num2
```

**Q33: How do I multiply two numbers?**

```kotlin
val result = num1 * num2
```

**Q34: How do I divide two numbers?**

```kotlin
val result = num1 / num2
```

**Q35: How do I calculate the remainder after division?**

```kotlin
val remainder = num1 % num2
```

</details>

<details>
<summary><h3>Conditionals</h3></summary>

**Q41: How do I display "Adult" if the age is at least 18?**

```kotlin
if (age >= 18) {
    textViewResult.text = "Adult"
}
```

**Q42: How do I display "Minor" if the age is below 18?**

```kotlin
if (age < 18) {
    textViewResult.text = "Minor"
}
```

**Q43: How do I display "Positive" or "Negative" based on a number?**

```kotlin
if (number >= 0) {
    textViewResult.text = "Positive"
} else {
    textViewResult.text = "Negative"
}
```

</details>

<details>
<summary><h3>Random Numbers</h3></summary>

**Q51: How do I generate a random number from 1 to 10?**

```kotlin
val randomNumber = (1..10).random()
```

**Q52: How do I simulate rolling a six-sided die?**

```kotlin
val roll = (1..6).random()
```

**Q53: How do I display a random lucky number when the user presses a button?**

```kotlin
buttonGenerate.setOnClickListener {
    val lucky = (1..100).random()
    textViewResult.text = lucky.toString()
}
```

</details>

</details>

<details>
<summary><h2>Flowcharts + Key</h2></summary>

<details>
<summary><h3>Flowchart Shape Key</h3></summary>

| Shape | Meaning | Kotlin Android examples |
| --- | --- | --- |
| `([ START / END ])` | **Oval / Terminator** | App/activity start or flow end |
| `[ Process ]` | **Rectangle** | Setup, variable creation, conversions, calculations |
| `[/ Input / Output /]` | **Parallelogram** | Reading `EditText`, displaying `TextView` |
| `{ Condition? }` | **Diamond** | `if` / `else` decisions |
| `↓` | **Arrow** | Flow direction |
| `⏸ WAIT` | **Event/Wait** | App waits for button click |

</details>

<details>
<summary><h3>Project 1 — Simple Greeting App</h3></summary>

<details>
<summary><h4>Text-Based Flowchart</h4></summary>

```
([ START ])
    ↓
[ Load activity_main.xml layout ]
    ↓
[ Connect EditText to editName ]
    ↓
[ Connect Button to buttonHello ]
    ↓
[ Connect TextView to textResult ]
    ↓
⏸ WAIT FOR BUTTON CLICK
    ↓
[ Button clicked ]
    ↓
[/ Read editName text /]
    ↓
[ Convert text to String ]
    ↓
[ Store String in name ]
    ↓
[ Create "Hello, $name!" ]
    ↓
[/ Display greeting in textResult /]
    ↓
⏸ WAIT FOR NEXT BUTTON CLICK
```

</details>

<details>
<summary><h4>Core Pattern</h4></summary>

```
APP START
  ↓
SET UP UI
  ↓
WAIT
  ↓
BUTTON CLICK
  ↓
INPUT → PROCESS → OUTPUT
  ↓
WAIT AGAIN
```

</details>
</details>

<details>
<summary><h3>Project 2 — Two Number Adder</h3></summary>

<details>
<summary><h4>Core Logic</h4></summary>

```
INPUT 1
  ↓
STRING → INT
  ↓
INPUT 2
  ↓
STRING → INT
  ↓
  ADD
  ↓
OUTPUT
```

</details>
</details>

<details>
<summary><h3>Project 3 — Even or Odd Checker</h3></summary>

<details>
<summary><h4>Core Logic</h4></summary>

```
      INPUT
        ↓
     CONVERT
        ↓
    number % 2
        ↓
     EVEN?
    ↙     ↘
  YES     NO
   ↓       ↓
 EVEN     ODD
```

The **diamond** is the important part: the program has to make a decision before determining the output.

</details>
</details>

<details>
<summary><h3>Project 4 — Random Dice Roller</h3></summary>

<details>
<summary><h4>Core Logic</h4></summary>

```
BUTTON CLICK
    ↓
RANDOM 1–6
    ↓
STORE ROLL
    ↓
DISPLAY ROLL
    ↓
WAIT
```

Notice there is **no decision diamond** in this project. It's simply an event → process → output application.

</details>
</details>

<details>
<summary><h3>Project 5 — Pass or Fail Checker</h3></summary>

The program checks whether `grade >= 70`, then displays `"Pass"` or `"Fail"`.

</details>

<details>
<summary><h3>Kotlin Android Master Flowchart</h3></summary>

These five projects introduce an important architectural pattern that differs from your CLI programs:

```
                ([ APP START ])
                      ↓
             [ LOAD XML LAYOUT ]
                      ↓
             [ CONNECT UI VIEWS ]
                      ↓
                 ⏸ WAIT
                      ↓
               [ USER ACTION ]
                      ↓
               [ EVENT FIRES ]
                      ↓
              [/ GET INPUT /]
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
                 ⏸
               WAIT
                  ↓
            [ NEXT EVENT ]
```

### The big conceptual difference

Your earlier CLI programs generally followed:

```
START
 ↓
INPUT
 ↓
PROCESS
 ↓
OUTPUT
 ↓
END
```

Kotlin Android introduces:

```
START
 ↓
SETUP UI
 ↓
WAIT
 ↓
EVENT
 ↓
INPUT
 ↓
PROCESS
 ↓
OUTPUT
 ↓
WAIT
 ↓
EVENT
 ↓
...
```

That's the beginning of **event-driven programming**.

| Project | Main concept |
| --- | --- |
| **1. Greeting App** | UI controls + button events + Strings |
| **2. Two Number Adder** | UI input + type conversion + arithmetic |
| **3. Even/Odd Checker** | UI input + modulo + decision |
| **4. Dice Roller** | Events + randomization + output |
| **5. Pass/Fail Checker** | Events + comparison + branching |

</details>

</details>

<details>
<summary><h2>Sample Projects</h2></summary>

<details>
<summary><h3>Project 1 — Simple Greeting App</h3></summary>

<details>
<summary><h4>Step 1 — Create the GUI (<code>activity_main.xml</code>)</h4></summary>

The layout contains a text input for the user's name, a button to trigger the greeting, and a text label to display the result.

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:padding="24dp">

    <!-- Input: User's name -->
    <EditText
        android:id="@+id/editName"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Enter your name"
        android:inputType="textPersonName" />

    <!-- Action: Generate greeting -->
    <Button
        android:id="@+id/buttonHello"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="Say Hello" />

    <!-- Output: Greeting message -->
    <TextView
        android:id="@+id/textResult"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginTop="16dp"
        android:text="Your greeting will appear here"
        android:textSize="20sp" />

</LinearLayout>
```

</details>

<details>
<summary><h4>Step 2 — Connect the GUI and implement the logic (<code>MainActivity.kt</code>)</h4></summary>

```kotlin
class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        // Connect XML controls to Kotlin variables
        val editName = findViewById<EditText>(R.id.editName)
        val buttonHello = findViewById<Button>(R.id.buttonHello)
        val textResult = findViewById<TextView>(R.id.textResult)

        // Run code when the button is clicked
        buttonHello.setOnClickListener {

            // Read the input
            val name = editName.text.toString()

            // Display the greeting
            textResult.text = "Hello, $name!"
        }
    }
}
```

Expected behavior: The user enters `Alex`, presses Say Hello, and sees `Hello, Alex!`.

</details>
</details>

<details>
<summary><h3>Project 2 — Two Number Adder</h3></summary>

<details>
<summary><h4>Step 1 — Create the GUI (<code>activity_main.xml</code>)</h4></summary>

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:padding="24dp">

    <!-- Input: First number -->
    <EditText
        android:id="@+id/editNum1"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Enter first number"
        android:inputType="numberSigned" />

    <!-- Input: Second number -->
    <EditText
        android:id="@+id/editNum2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Enter second number"
        android:inputType="numberSigned" />

    <!-- Action: Add the numbers -->
    <Button
        android:id="@+id/buttonAdd"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="Add Numbers" />

    <!-- Output: Sum -->
    <TextView
        android:id="@+id/textAnswer"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginTop="16dp"
        android:text="Answer will appear here"
        android:textSize="20sp" />

</LinearLayout>
```

</details>

<details>
<summary><h4>Step 2 — Connect the GUI and implement the logic (<code>MainActivity.kt</code>)</h4></summary>

```kotlin
class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        // Connect XML controls
        val editNum1 = findViewById<EditText>(R.id.editNum1)
        val editNum2 = findViewById<EditText>(R.id.editNum2)
        val buttonAdd = findViewById<Button>(R.id.buttonAdd)
        val textAnswer = findViewById<TextView>(R.id.textAnswer)

        buttonAdd.setOnClickListener {

            // Read and convert both inputs
            val num1 = editNum1.text.toString().toInt()
            val num2 = editNum2.text.toString().toInt()

            // Calculate the sum
            val sum = num1 + num2

            // Display the answer
            textAnswer.text = sum.toString()
        }
    }
}
```

Expected behavior: Enter `5` and `7`, press Add Numbers, and see `12`.

</details>
</details>

<details>
<summary><h3>Project 3 — Even or Odd Checker</h3></summary>

<details>
<summary><h4>Step 1 — Create the GUI (<code>activity_main.xml</code>)</h4></summary>

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:padding="24dp">

    <!-- Input: Number to check -->
    <EditText
        android:id="@+id/editNumber"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Enter an integer"
        android:inputType="numberSigned" />

    <!-- Action: Check the number -->
    <Button
        android:id="@+id/buttonCheck"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="Check Even or Odd" />

    <!-- Output: Result -->
    <TextView
        android:id="@+id/textResult"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginTop="16dp"
        android:text="Result will appear here"
        android:textSize="20sp" />

</LinearLayout>
```

</details>

<details>
<summary><h4>Step 2 — Connect the GUI and implement the logic (<code>MainActivity.kt</code>)</h4></summary>

```kotlin
class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        // Connect XML controls
        val editNumber = findViewById<EditText>(R.id.editNumber)
        val buttonCheck = findViewById<Button>(R.id.buttonCheck)
        val textResult = findViewById<TextView>(R.id.textResult)

        buttonCheck.setOnClickListener {

            // Read the input
            val number = editNumber.text.toString().toInt()

            // Determine whether the number is even or odd
            if (number % 2 == 0) {
                textResult.text = "Even"
            } else {
                textResult.text = "Odd"
            }
        }
    }
}
```

Expected behavior: Enter `8` and see `Even`. Enter `7` and see `Odd`.

</details>
</details>

<details>
<summary><h3>Project 4 — Random Dice Roller</h3></summary>

<details>
<summary><h4>Step 1 — Create the GUI (<code>activity_main.xml</code>)</h4></summary>

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:gravity="center"
    android:padding="24dp">

    <!-- Output: Dice roll -->
    <TextView
        android:id="@+id/textRoll"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center"
        android:text="Roll the dice!"
        android:textSize="32sp"
        android:layout_marginBottom="24dp" />

    <!-- Action: Generate a random number -->
    <Button
        android:id="@+id/buttonRoll"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="Roll Dice" />

</LinearLayout>
```

</details>

<details>
<summary><h4>Step 2 — Connect the GUI and implement the logic (<code>MainActivity.kt</code>)</h4></summary>

```kotlin
class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        // Connect XML controls
        val buttonRoll = findViewById<Button>(R.id.buttonRoll)
        val textRoll = findViewById<TextView>(R.id.textRoll)

        buttonRoll.setOnClickListener {

            // Generate a random integer from 1 through 6
            val roll = (1..6).random()

            // Display the result
            textRoll.text = roll.toString()
        }
    }
}
```

Expected behavior: Press Roll Dice to generate and display a random number between `1` and `6`.

</details>
</details>

<details>
<summary><h3>Project 5 — Pass or Fail Checker</h3></summary>

<details>
<summary><h4>Step 1 — Create the GUI (<code>activity_main.xml</code>)</h4></summary>

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:padding="24dp">

    <!-- Input: Student grade -->
    <EditText
        android:id="@+id/editGrade"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Enter grade (0-100)"
        android:inputType="number" />

    <!-- Action: Evaluate grade -->
    <Button
        android:id="@+id/buttonCheck"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="Check Grade" />

    <!-- Output: Pass or fail -->
    <TextView
        android:id="@+id/textResult"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginTop="16dp"
        android:text="Result will appear here"
        android:textSize="20sp" />

</LinearLayout>
```

</details>

<details>
<summary><h4>Step 2 — Connect the GUI and implement the logic (<code>MainActivity.kt</code>)</h4></summary>

```kotlin
class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        // Connect XML controls
        val editGrade = findViewById<EditText>(R.id.editGrade)
        val buttonCheck = findViewById<Button>(R.id.buttonCheck)
        val textResult = findViewById<TextView>(R.id.textResult)

        buttonCheck.setOnClickListener {

            // Read and convert the grade
            val grade = editGrade.text.toString().toInt()

            // Compare the grade against the passing threshold
            if (grade >= 70) {
                textResult.text = "Pass"
            } else {
                textResult.text = "Fail"
            }
        }
    }
}
```

</details>
</details>

</details>