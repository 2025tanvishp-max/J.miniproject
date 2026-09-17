🎯 QuizApp – Java Mini Project

A simple console-based quiz application built using Java.
The application allows users to select a difficulty level and answer randomly selected questions while keeping track of their score.

👨‍🎓 Student Details

Detail

Information

Name

Tanvish Poojari

Roll No.

203

Division / Cohort

Demiz Hassabis

Project Name

QuizApp

Technology

Java

Application Type

Console-based Quiz Application

📌 Project Overview

QuizApp is a Java-based console application designed to demonstrate fundamental Java programming concepts through an interactive quiz.

The user can choose between three difficulty levels:

🟢 Easy

🟡 Medium

🔴 Hard

After selecting a difficulty, the program randomly selects 3 questions from that difficulty level. The user answers each question using A, B, or C.

The application checks the answers, maintains the score, and displays the final score and percentage.

🎯 Objectives

Develop an interactive quiz application using Java.

Store quiz questions, options, difficulty levels, and correct answers in a structured two-dimensional array.

Allow the user to choose a difficulty level using switch-case.

Randomly select questions while avoiding repeated questions.

Accept and validate user answers using String methods.

Maintain the user's score and calculate the final percentage.

Demonstrate core Java programming concepts in a practical mini project.

🔍 Scope

The current scope of QuizApp includes:

Three difficulty levels: Easy, Medium, and Hard.

Three questions per quiz attempt.

Random question selection.

Prevention of duplicate questions during the same attempt.

Multiple-choice questions with three options.

Automatic answer checking.

Score calculation.

Percentage calculation.

Console-based user interaction.

The questions and answers are currently stored directly inside the Java program.

🧠 Concepts Used

Concept

Use in QuizApp

Class

QuizApp contains the application logic.

Objects

Scanner, Random, and ArrayList are used as objects.

Scanner

Reads user input from the console.

Two-Dimensional Array

String[][] q stores difficulty, question, options, and correct answer.

Variables & Data Types

int and String are used for numeric and text data.

Switch-Case

Selects Easy, Medium, or Hard difficulty.

If-Else

Checks whether the entered answer is correct.

For Loop

Repeats the quiz process three times.

Do-While Loop

Generates a valid random question.

Random

Generates random question indexes.

ArrayList

Stores used question indexes to prevent repetition.

Methods

quiz() separates quiz processing from main().

Parameter & Return Value

String level passes difficulty and return score sends the result back.

String Methods

toUpperCase() and equals() process and compare answers.

Operators

Arithmetic, logical, comparison, and increment operators are used.

Static

Allows class-level access to shared members.

⚙️ How the Program Works

Start
  ↓
Display Quiz Menu
  ↓
Select Difficulty
  ↓
Switch-Case
  ↓
Call quiz(difficulty)
  ↓
Generate Random Question
  ↓
Check Difficulty
  ↓
Check Duplicate
  ↓
Display Question & Options
  ↓
User Enters Answer
  ↓
Check Answer
  ↓
Update Score
  ↓
Repeat 3 Times
  ↓
Return Score
  ↓
Calculate Percentage
  ↓
Display Result
  ↓
End

🗃️ Question Data Structure

Each question is stored as one row in the two-dimensional array q.

Index

Stores

0

Difficulty

1

Question

2

Option A

3

Option B

4

Option C

5

Correct Answer

Example:

{"Easy", "Which keyword creates a class?", "class", "object", "new", "A"}

🔑 Key Code Logic

Random question selection

Random r = new Random();
n = r.nextInt(q.length);

Preventing duplicate questions

ArrayList<Integer> used = new ArrayList<>();

do {
    n = r.nextInt(q.length);
} while (!q[n][0].equals(level) || used.contains(n));

used.add(n);

Checking the answer

String ans = sc.next().toUpperCase();

if (ans.equals(q[n][5])) {
    System.out.println("Correct!");
    score++;
} else {
    System.out.println("Wrong! Answer: " + q[n][5]);
}

Calculating percentage

(score * 100 / 3.0)

📸 Project Screenshots

💻 QuizApp Source Code — Part 1



💻 QuizApp Source Code — Part 2



🖥️ QuizApp Console Output



💻 Sample Output

===== JAVA QUIZ =====
1. Easy
2. Medium
3. Hard
Choose: 1

Which symbol ends a statement?
A. :
B. ;
C. .
Answer: a
Wrong! Answer: B

Which keyword creates a class?
A. class
B. object
C. new
Answer: b
Wrong! Answer: A

Which type stores whole numbers?
A. double
B. int
C. char
Answer: a
Wrong! Answer: B

===== RESULT =====
Difficulty: Easy
Score: 0/3
Percentage: 0.0%

📁 Project Structure

QuizApp/
│
├── QuizApp.java
├── QuizDifficulty.java
├── README.md
├── QuizApp_Mini_Project_Report.pdf
└── screenshots/
    ├── quizapp-code-part-1.png
    ├── quizapp-code-part-2.png
    └── quizapp-output.png

▶️ How to Run

1. Clone the Repository

git clone <repository-url>

2. Open the Project

Open the project folder in VS Code or another Java-supported IDE.

3. Compile the Program

javac QuizApp.java

4. Run the Program

java QuizApp

🛠️ Technologies Used

Java

Java Collections

Java Scanner

Java Random

Java ArrayList

VS Code

Terminal

🚀 Future Enhancements

Possible future improvements include:

More questions.

More answer options.

Timer-based quizzes.

High-score tracking.

Different quiz categories.

Graphical User Interface (GUI).

Saving quiz results to a file or database.

User login and player profiles.

📄 Documentation

Detailed project documentation is available in:

QuizApp_Mini_Project_Report.pdf

The report contains the project overview, objectives, scope, concepts used, working process, data structure, key code logic, and conclusion.

👨‍💻 Author

Tanvish Poojari
Roll No.: 203
Division / Cohort: Demiz Hassabis

⭐ QuizApp – A Java Mini Project


CODE-
<img width="1470" height="956" alt="Screenshot 2026-09-17 at 5 25 06 PM" src="https://github.com/user-attachments/assets/d35ab879-3e64-421e-a863-704521a429a8" />
<img width="1470" height="956" alt="Screenshot 2026-09-17 at 5 25 01 PM" src="https://github.com/user-attachments/assets/4e1ea07a-763e-4119-9f98-8cfae42de403" />

OUTPUT-
<img width="1470" height="956" alt="Screenshot 2026-09-17 at 5 25 29 PM" src="https://github.com/user-attachments/assets/4b26d8a3-30f3-4e3e-8fcc-5bdcd1dd4d04" />
