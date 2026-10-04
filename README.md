# CodeClarity AI - Code Review Interface

## Project Overview

CodeClarity AI is an automated code-review system that analyzes source code and identifies potential bugs, coding issues, severity levels, and possible improvements.

This project extends the CodeClarity AI system by providing an interactive Code-Review Interface using Gradio. Users can enter source code, select the programming language, and receive an automated code-review report.

## Problem Statement

Develop a code-review interface that allows users to submit source code and automatically receive information about potential bugs, severity, explanations, code-quality score, and improvement suggestions.

## Objectives

* Provide an easy-to-use code-review interface.
* Allow users to enter source code directly.
* Support multiple programming languages.
* Detect common programming issues.
* Classify detected issues according to severity.
* Explain the detected problems.
* Generate code-improvement suggestions.
* Calculate an overall code-quality score.
* Display the review results in an interactive interface.

## Features

* Interactive code editor
* Programming language selection
* Automated bug detection
* Bug severity classification
* Bug explanation
* Code-improvement suggestions
* Code-quality score
* Risk-level classification
* Interactive Gradio interface
* Google Colab support

## Supported Programming Languages

The current interface supports:

* Python
* Java
* C
* C++

## Technologies Used

* Python
* Google Colab
* Gradio
* Regular Expressions
* Rule-Based Code Analysis

## System Workflow

```text
User
  |
  v
Enter Source Code
  |
  v
Select Programming Language
  |
  v
Code Review Engine
  |
  +----------------------+
  |                      |
  v                      v
Bug Detection       Code Analysis
  |                      |
  v                      v
Severity Analysis   Quality Analysis
  |                      |
  +----------+-----------+
             |
             v
     Improvement Suggestions
             |
             v
       Quality Score
             |
             v
        Review Report
```

## Project Structure

```text
CodeClarity-AI-Code-Review/
│
├── CodeClarity_Code_Review_Interface.ipynb
├── README.md
└── requirements.txt
```

## Installation

Install the required Python package:

```bash
pip install gradio
```

Or, in Google Colab:

```python
!pip install -q gradio
```

## How to Run

### Step 1: Open Google Colab

Upload the following notebook:

```text
CodeClarity_Code_Review_Interface.ipynb
```

### Step 2: Run All Cells

Execute the notebook cells in order.

### Step 3: Open the Interface

After executing the final cell, Gradio generates a temporary public URL.

Example:

```text
 Running on public URL: https://1e327c2c2a756db31d.gradio.live
```

Open the generated URL to access the Code-Review Interface.

## How to Use the Interface

1. Select the programming language.
2. Enter or paste the source code.
3. Click the **Review Code** button.
4. The system analyzes the source code.
5. View the detected bugs.
6. Check the severity of each issue.
7. Read the explanation.
8. Review the improvement suggestions.
9. Check the overall code-quality score and risk level.

## Example Input

```python
def calculate_average(numbers):
    total = sum(numbers)
    return total / len(numbers)

numbers = []

password = "admin123"

print(calculate_average(numbers))
```

## Example Analysis

The system can identify potential issues such as:

### Bug 1

```text
Type: Division by Zero
Severity: HIGH
```

Explanation:

```text
The code may attempt to divide by zero when the list is empty.
```

### Bug 2

```text
Type: Hardcoded Credential
Severity: HIGH
```

Explanation:

```text
A password appears to be hardcoded in the source code.
```

## Improvement Suggestions

The system may recommend:

```text
1. Check the denominator before performing division.

2. Store credentials securely using environment variables
   or a secret manager.

3. Follow appropriate coding and formatting conventions.
```

## Code Quality Score

The system calculates a score based on the detected issues.

```text
80 - 100  : GOOD
60 - 79   : MEDIUM RISK
0 - 59    : HIGH RISK
```

## Output

The Code-Review Interface provides:

```text
Code Review Summary
        |
        +-- Programming Language
        |
        +-- Number of Bugs
        |
        +-- Code Quality Score
        |
        +-- Risk Level
        |
        +-- Bug Detection
        |
        +-- Severity
        |
        +-- Bug Explanation
        |
        +-- Improvement Suggestions
```

## Current Limitations

* The current version uses rule-based analysis.
* It detects predefined/common coding issues.
* It does not perform complete semantic analysis.
* The Gradio public URL generated from Google Colab is temporary.
* The current version does not automatically modify the submitted code.

## Future Enhancements

* Integrate an LLM for advanced code analysis.
* Add static-analysis tools such as Bandit and Radon.
* Support additional programming languages.
* Detect more security vulnerabilities.
* Add code-complexity analysis.
* Generate corrected code automatically.
* Generate downloadable review reports.
* Store previous code-review results.
* Integrate with GitHub repositories.
* Add authentication and user history.
* Deploy the interface permanently using Hugging Face Spaces.

## Conclusion

CodeClarity AI - Code Review Interface provides an interactive solution for automated source-code analysis. It combines bug detection, severity classification, explanations, improvement suggestions, and quality scoring into a single user-friendly interface.

The system can be further extended with AI-based analysis and static-analysis tools to provide more accurate and comprehensive code reviews.

## Author

DHARSHINI A
