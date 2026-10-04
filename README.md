# CodeClarity AI – Code Review Interface

## Project Overview

CodeClarity AI is an automated code-review system designed to analyze source code and identify potential programming issues.

The Code-Review Interface provides a simple web-based interface where users can submit source code and receive an automated review.

## Features

* Source code input
* Programming language selection
* Automated bug detection
* Bug severity classification
* Bug explanations
* Code improvement suggestions
* Code quality score
* Risk-level classification
* Interactive Gradio interface

## Supported Languages

* Python
* Java
* C
* C++

## Technologies Used

* Python
* Google Colab
* Gradio
* Regular Expressions
* Rule-based Code Analysis

## System Workflow

```text
User
  ↓
Enter Source Code
  ↓
Select Programming Language
  ↓
Code Review Engine
  ↓
Bug Detection
  ↓
Severity Analysis
  ↓
Improvement Suggestions
  ↓
Quality Score
  ↓
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

## How to Run

### Step 1: Open Google Colab

Upload:

```text
CodeClarity_Code_Review_Interface.ipynb
```

### Step 2: Install Dependencies

Run:

```python
!pip install -q gradio
```

### Step 3: Run the Notebook

Execute all cells in order.

The Gradio interface will generate a temporary public URL.

## Example

Example input:

```python
def calculate_average(numbers):
    total = sum(numbers)
    return total / len(numbers)

numbers = []

password = "admin123"

print(calculate_average(numbers))
```

The system can identify issues such as:

* Possible division by zero
* Hardcoded credentials
* Input validation issues

It then provides improvement suggestions and a code-quality score.

## Output

The interface provides:

```text
Code Review Summary
Bug Detection
Severity
Bug Explanation
Improvement Suggestions
Code Quality Score
Risk Level
```

## Future Enhancements

* AI/LLM-based code analysis
* Support for additional programming languages
* Code complexity analysis
* Security vulnerability detection
* Automated code fixing
* Downloadable review reports
* GitHub repository integration

## Author

DHARSHINI A
