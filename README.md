# Computational Theory

## 1. Project Overview

This repository contains my submission for the **Computational Theory** assessment for *Winter 2025/26.*
The work focuses on implementing and analysing core components of the **Secure Hash Standard (FIPS 180-4)** using *Python* and *NumPy*, supported by clear explanations, reproducible code, and ongoing revision through consistent commits.

The assessment requires all problems to be completed in one **Jupyter notebook** called ``problems.ipynb``. This notebook needs to be organised in a way suitable for review and testing. It also must maintain consistent version control and structure.

The structure and requirements of this project follow the official assessment instructions and guidance provided by the module’s [GitHub repository](https://github.com/ianmcloughlin/computational-theory/tree/main).

### Purpose of Project

The primary goal of this project is to demonstrate a strong practical **understanding of the computational and mathematical foundations** behind the **SHA-256 hashing algorithm**, including:

- Binary word operations

- Bitwise functions and rotation logic

- Prime-based constant derivation

- Cryptographic padding rules

- Block-based message processing

- Iterative hash computation and compression functions

- Password hashing, weaknesses, and mitigation strategies

The project goes beyond simply solving each question: it **documents the theory behind each concept**, applies testing, references appropriate sources, and structures the work so it can be rerun cleanly on any machine.

## 2. Respository Structure
The project structure is quite simple and only contains the ``README.md`` and the ``problems.ipynb``. My repository also contains a .``vscode`` file which just contains JSON settings configuration file but it is not particularly relevant to this assignment.
```
computational-theory/
│
├── problems.ipynb              
├── README.md                
```


## 3. How to Run the Notebooks

To run `problems.ipynb`, clone the repository and set up a Python environment with the required dependencies.

### 1. Clone the Repository
**With HTTPS:** 
```
git clone https://github.com/fionnmcgoldrick123/computational-theory.git
cd computational-theory
```

**With SSH:**
```
git clone git@github.com:fionnmcgoldrick123/computational-theory.git
cd computational-theory
```

### 2. Create and Activate a Virtual Environment
It is recommended to use a virtual environment to keep dependencies isolated.
```
python3 -m venv venv
source venv/bin/activate        # macOS / Linux
venv\Scripts\activate           # Windows
```

### 3. Install Dependencies
Install NumPy dependency.
```
pip install numpy
```

### 4. Open the Project in Visual Studio Code
```
code . 
```

### 5. Select your Python Interpreter
**In Visual Studio Code:**

1. Press **Ctrl+Shift+P**
2. Type **Python: Select Interpreter**
3. Choose the interpreter from your ``.venv`` folder

This ensures the notebook uses the correct environment.

### 6. Run the Notebook

Open ``problems.ipynb`` and click the run / play button on any given cell.

**NOTE:** *Ensure the first cell containing the NumPy import is run before executing later cells.*

## 4. Dependencies

This project requires only one external **Python** package: **NumPy**.

### Required Packages:
- **NumPy** — used for 32-bit integer operations, bitwise functions, and numerical calculations required by the Secure Hash Standard.

**Install using:**

```
pip install numpy
```

## 5. Resources & References

This section contains each source that I used both universally throughout the assignment, and the ones I used for each individual problem.

### Universal References

### Problem 1 References

### Problem 2 References

### Problem 3 References

### Problem 4 References

### Problem 5 References

## 6. Assessment Requirements Checklist

## 7. Testing / Verification Notes

## 8. Author
This repo was designed by *Fionn McGoldrick*.

G00422349@atu.ie

