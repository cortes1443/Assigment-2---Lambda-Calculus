# Lambda Calculus - LambdaShell

## Students
- Juan Cortes
- Santiago Arellano

## Environment and Tool Versions

This project was developed and tested using the following setup:

**Operating System (Host):**
- Microsoft Windows [Version 10.0.19045.5737]

**Windows Subsystem for Linux (WSL):**
- WSL Version: 2.4.13.0  
- Kernel Version: 5.15.167.4-1  
- WSLg Version: 1.0.65  
- MSRDC Version: 1.2.5716  
- Direct3D: 1.611.1.81528511  
- DXCore: 10.0.22000.1-240331-1435.ge-release  
- Windows Build: 10.0.19045.5737

**Linux Distribution:**
- Debian (via WSL)

**Compiler:**
- GHC (The Glorious Glasgow Haskell Compilation System), version 9.12.2

**LambdaShell:**
- Version: 0.9.9.1  
- Author: Robert Dockins

## Combinators and Their Purpose

These are the main combinators defined in `ldefs.lambda`:

- **TRUE** – Represents the boolean value true (returns first value).
- **FALSE** – Represents the boolean value false (returns second value).
- **PAIR** – Constructs a pair from two values.
- **FST** – Retrieves the first element of a pair.
- **SND** – Retrieves the second element of a pair.
- **ZERO** – Represents the Barendregt’s numeral 0 (Identity combinator).
- **SUCC** – Returns the successor of a Barendregt’s number  (adds 1).
- **PRED** – Represents the predecessor (subtracts 1).
- **ISZERO** – Checks whether a Barendregt’s numeral is zero.
- **ONE, TWO, THREE, FOUR, FIVE** – Barendregt’s numerals for 1 through 5.

These building blocks allow construction of logic and arithmetic purely through lambda abstraction and application.

## How to Run the Project

1. **Open your terminal in Windows and enter the Debian environment:**
   ```bash
   wsl -d Debian
   ```

2. **Navigate to the directory where the lambda definitions file is located:**
   Example:
   ```bash
   cd /mnt/c/Users/juanc/
   ```

3. **Start LambdaShell:**
   ```bash
   lambdaShell
   ```

4. **Load the lambda definitions file:**
   ```lambdashell
   :load ldefs.lambda
   ```
   
5. **Visualize expressions:**
   You can see all the combinators in the file by using showall:
   ```lambdashell
   :showall
   ```
   
6. **Evaluate lambda expressions:**
   Once loaded, you can type in expressions to reduce them. Examples:
   ```lambdashell
   PRED ONE
   ISZERO ZERO
   SUCC THREE
   ```

## References

- ChatGPT – Used for assistance with LambdaShell usage instructions.
- LambdaShell GitHub Repository – https://github.com/robertdockins/lambdashell


This project demonstrates lambda calculus concepts using the LambdaShell interpreter in a WSL environment. By defining and testing core combinators, we simulate basic logic and arithmetic purely through function abstraction and application.
