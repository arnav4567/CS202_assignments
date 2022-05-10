# Assignment 2 (SAT Solver)

## Problem Statement

Implement a **SAT solver**. Given a formula in the **DIMACS representation**, your implementation should return:

1) a model if the formula is satisfiable

2) report that the formula is unsatisfiable

You are free to use any language and algorithm (Semantic Tableau, Analytic Tableau, DPLL or a combination).

### **Deliverables**
The source code of your implementation. <br>
A brief report (less than 5-pages) describing your implementation, assumptions, and limitations.<br>
A set of test cases (at least 5) with the expected output. (tests folder).

The quality of all the above would affect your marks. 

### **Submission Format**

Your submission MUST be in the following format:

The submission should be a zip file.
The zip file should be named as assignment_"number"_"Roll-of-student1"_"Roll-of-student2".
Zip the content of the source as is and submit. 

### **Some important comments**
Before doing anything "extra" (which might fetch bonus marks), first, complete the basic expectations from your implementation.
Programs are expected to display their results in a user-friendly manner; a user would never like to use a program that simply spits out a bunch of numbers. So, display the results from your programs suitably.

<br>
<br>

## Description of submitted files

The DPLL algorithm has been used to implement the SAT Solver. The code is contained in the [satSolver.py](/Assignment_2/satSolver.py) file.

Simply run the file through terminal or any suitable Python IDE. After running the file, enter the path of the test case
which contains the cnf file to be tested.

If the model is unsatisfiable, the output contains a single line "UNSAT". Else, the output displays the model.

The test cases that we have provided are present in the [testcases](/Assignment_2/testcases/) folder. The expected outputs for those test cases are also present in the same folder.

The implementation details, approach, pseudocodes, function details, assumptions and limitations are included in the [CS202_A2_Report.pdf](/Assignment_2/CS202_A2_report.pdf) file.

If the user wants to test some other formula, the path to that file must be given. Additionally, the output will be stored in the text file **outfile.txt**, which is present in the same directory as the .py file.