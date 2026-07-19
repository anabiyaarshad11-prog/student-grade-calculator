# student-grade-calculator
# Student Grade Calculator

**DecodeLabs | Project 2 — Computational Phase**

A Java console application that processes a student's marks across multiple subjects and generates a performance report: total marks, average percentage, and a final letter grade.

## Overview

This project focuses on core programming fundamentals rather than complex architecture:
- Taking multiple user inputs
- Performing arithmetic operations (totals, averages)
- Using conditional branching to classify data
- Displaying results in a clear, readable format

## Features

- Accepts marks (out of 100) for any number of subjects
- Validates input so marks stay within the 0–100 range
- Calculates:
  - Total marks scored
  - Average percentage
- Assigns a letter grade based on the average:

  | Average % | Grade |
  |-----------|-------|
  | 90–100    | A     |
  | 80–89     | B     |
  | 70–79     | C     |
  | 60–69     | D     |
  | 50–59     | E     |
  | Below 50  | F     |

- Displays a formatted report listing each subject's marks alongside the total, average, and final grade

## Requirements

- Java Development Kit (JDK) 8 or later
- A terminal, or an IDE such as VS Code with the **Extension Pack for Java** installed

## Project Structure

```
StudentGradeCalculator/
├── StudentGradeCalculator.java   # Main application source file
├── README.md                     # Project documentation
└── .vscode/
    └── launch.json               # VS Code run/debug configuration (optional)
```

## How to Run

### Option 1: Command line

```bash
javac StudentGradeCalculator.java
java StudentGradeCalculator
```

### Option 2: VS Code

1. Open the project folder in VS Code (**File → Open Folder**).
2. Make sure the **Extension Pack for Java** is installed.
3. Open `StudentGradeCalculator.java`.
4. Click the **Run** link above `public static void main(...)`, or press `F5`.

If you use a `launch.json`, set `"console": "integratedTerminal"` so the Scanner-based input prompts work correctly.

## Sample Run

```
Enter number of subjects: 3
Enter name for subject 1: Math
Enter marks for Math (out of 100): 92
Enter name for subject 2: Physics
Enter marks for Physics (out of 100): 78
Enter name for subject 3: English
Enter marks for English (out of 100): 85

========== STUDENT GRADE REPORT ==========
Math                 : 92.00 / 100
Physics              : 78.00 / 100
English              : 85.00 / 100
-------------------------------------------
Total Marks         : 255.0 / 300
Average Percentage   : 85.00%
Final Grade          : B
===========================================
```

## Core Concepts Demonstrated

- **Variables & arrays** — storing subject names and marks
- **Loops** — collecting input and rendering the report
- **Arithmetic operations** — totals and averages
- **Conditional statements** — grade classification logic

## Notes / Possible Extensions

- Adjust the grading scale in the `if/else if` block if your institution uses different cutoffs.
- Could be extended to support weighted subjects (credit hours), GPA calculation, or exporting the report to a file.

## Author

Java Developer, DecodeLabs — Project 2 Submission
