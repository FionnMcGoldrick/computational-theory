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

- [Computational Theory GitHub Repo](https://github.com/ianmcloughlin/computational-theory) - *Base resource for the notebook. Used for understanding the notebook and problem requirements. Also, for notes on understanding many concepts relevant to this notebook.*  

- [NIST (Secure Hash Standard)](https://csrc.nist.gov/pubs/fips/180-2/final) - *Used for getting the necessary formulas to complete the problems.* 

- [NumPy Docs](https://numpy.org/doc/) - *Used to understand NumPy functionalities, use cases, and also for NumPy syntax.*

- [numpydoc](https://numpydoc.readthedocs.io/en/latest/format.html) - *Helpful for planning out Docstring structure*

- [Real Python](https://realpython.com/) - *Used for understanding new Python concepts I was not aware of.*

- [SHA: Secure Hashing Algorithm - Computerphile](https://www.youtube.com/watch?v=DMtFhACPnTY) - *YouTube video used for understang SHA general knowledge.*

- [W3Schools - Python](https://www.w3schools.com/python/) - *Used for understanding anything python. Syntax, built-in functions, data structures, ect...*

- [ChatGPT](https://chatgpt.com/) - *Used for a personalised explanation of concepts that I could not find helpful sources on. Also used for assistance with grammar, spelling mistakes, and scientific structure in the markdown.*

- [Claude](https://claude.ai/new) - *Used for help in debugging Python code if I could not find the issues myself or online.*

- [StackOverflow](https://stackoverflow.com/questions) - *Often used to find correct or improved implementations of my code.* 

- [Sha Algorithm - Visualisation](https://sha256algorithm.com/) - *Massive help for visualising SHA-256 concepts.*

### Problem 1 References

- [Bitwise Operators in Python](https://realpython.com/python-bitwise-operators/) - *To get a understand bitwise operations further.*

- [Bitwise Operation](https://en.wikipedia.org/wiki/Bitwise_operation) - *To obtain a deeper understanding of bitwise operations.*

### Problem 2 References

- [List of prime numbers](https://en.wikipedia.org/wiki/List_of_prime_numbers) - *Used for reaffirming prime function output.*

- [Cuberoot Root Calculator](https://www.calculatorsoup.com/calculators/algebra/cuberoots.php) - *Checking if function outputting correct primes.*

- [Cuberoot Wikepedia](https://en.wikipedia.org/wiki/Cube_root) - *Information on cuberoots*

- [How to represent fractional numbers in Binary](https://www.luisllamas.es/en/represent-fractional-numbers-in-binary/) - *Used for understanding how to represent fractional numbers in binary.*

- [Hexadeximal Wiki](https://en.wikipedia.org/wiki/Hexadecimal) - *Information on hexadecimal representation* 

### Problem 3 References

- [Real Python - Generators](https://realpython.com/introduction-to-python-generators/) - *Used to better understand how generators work and their applications.*

- [Real Python - Byte Objects](https://realpython.com/python-bytes/) - *Understand byte object better.*

- [MojoAuth - MD5 vs MD4](https://mojoauth.com/compare-hashing-algorithms/) - *Researching MD5 & MD4 cryptographic functions.* 

- [Wikipedia - Guido van Rossum](https://en.wikipedia.org/wiki/Guido_van_Rossum) - *Researching Python history for discussion section.*

- [Python Enhancement Proposals](https://peps.python.org/pep-0225/) - *Used for understanding the PEP 225 proposals for the discussion section.*

- [Wikipedia - Endianness](https://en.wikipedia.org/wiki/Endianness) - *For understanding endianness.*

- [W3Schools - Python Built in Functions](https://www.w3schools.com/python/python_ref_functions.asp) - *For finding functions I will need for this problem and how they work.*

### Problem 4 References

- [Hash function](https://en.wikipedia.org/wiki/Hash_function) - *Better understanding of hash functions.*

- [SHA-256 | COMPLETE Step-By-Step Explanation - RedBlockBlue](https://www.youtube.com/watch?v=orIgy2MjqrA) - *Useful YouTube video. Watched onward from **4:27** for this problem.*

- [CS255 - Stanford: Introduction to Cryptography](https://crypto.stanford.edu/~dabo/cs255/) - *Taught how iterative hashing worked and why internal state is updated block by block*

- [SHA256 - Online Tools](https://emn178.github.io/online-tools/sha256.html) - *Used for visualisation of hashing and experimenting with input and hashed output. Also used to test my implementation functionality.*

- [Simplil Learn: A Definitive Guide to Learn The SHA-256 (Secure Hash Algorithms)](https://www.simplilearn.com/tutorials/cyber-security-tutorial/sha-256-algorithm) - *Extremely good graphics for explaining hashing and SHA-256 concepts.*

### Problem 5 References

- [UTF-8 - Wikepedia](https://en.wikipedia.org/wiki/UTF-8) - *To consolidate my understanding of the UTF-8 format*

- [UTF-8, Explained Simply - Nic Barker](https://www.youtube.com/watch?v=vpSkBV5vydg) - *More theory and background behind UTF-8 encoding*

- [The Unicode Standard](https://www.unicode.org/standard/standard.html) - *Used for learning about the Unicode Standard deeper*

- [ASCII Code](https://www.ascii-code.com/) - *To compare UTF-8 to ASCII encoding*

- [Nord Pass](https://nordpass.com/most-common-passwords-list/) - *For finding a list of the top 200 most common passwords*

- [Real Python - hashlib](https://realpython.com/ref/stdlib/hashlib/#:~:text=The%20Python%20hashlib%20module%20provides,%2C%20password%20storage%2C%20and%20more.) - *Researching libraries to help with this problem*

## 6. Assessment Requirements Checklist

## 7. Testing / Verification Notes

## 8. Author
This repo was designed and written by *Fionn McGoldrick*.

G00422349@atu.ie

