# Assignment 1 (Sudoku Solver and Generator)

## Problem Statement

This assignment has two questions to be solved. You are expected to submit code for both Q1 & Q2. 
You should also submit a brief write-up on your approach to solving these questions.

In this question, you have to write a k-sudoku puzzle pair solver and generator by encoding the problem to **propositional logic** and solving it via a SAT solver (https://pysathq.github.io/). 

Given a sudoku puzzle pair **S1, S2** (both of dimension k) as input, your job is to write a program to fill the empty cells of both sudokus such that it satisfies the following constraints :
+ Individual sudoku properties should hold.
+ For each empty cell **S1[i, j] ≠ S2[i, j]**, where i is row and j is column.

**Input**: Parameter **k**, single CSV file containing two sudokus. The first **k<sup>2</sup>** rows are for the first sudoku and the rest are for the second sudoku. Each row has **k<sup>2</sup>** cells. Each cell contains a number from **1** to **k<sup>2</sup>**. Cell with **0** specifies an empty cell.

**Output**: If the sudoku puzzle pair doesn't have any solution, you should return **None** otherwise return the filled sudoku pair.


In the second part, you have to write a k-sudoku puzzle pair generator. The puzzle pair must be maximal (have the largest number of holes possible) and must have a unique solution. 

**Input**: Parameter k

**Output**: CSV file containing two sudokus in the format mentioned in Q1.

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

## Description of submittted files
+ The codes for both Q1 and Q2 are present in the [codes](/Assignment_1/codes/) folder. Q1(solver) - [a1q1_sudoku_solver.py](/Assignment_1/codes/a1q1_sudoku_solver.py). Q2(generator) - [a1q2_sudoku_generator.py](/Assignment_1/codes/a1q2_sudoku_generator.py)
+ The approach, implementation, limitations, and assumptions used while implementing the code has been included in the [report](/Assignment_1/report/CS202A1_report.pdf).
+ Tests have been included in the [tests](/Assignment_1/tests/) folder. They have been described in detail below.
+ Screenshots of some tests are also inside the [tests](/Assignment_1/tests/ExpectedOutputs.pdf) folder.

## Test cases description

6 cases have been included for Q1 in the [tests/q1](/Assignment_1/tests/q1/) folder.

Name of the file | Solution Exists | Remarks
--- | --- | --- |
ex1.csv (k=3) | Yes | 
ex2.csv (k=3) | No | This test has been included to check whether the code works for invalid inputs (when one or more entries in both the sudokus are common). |
ex3.csv (k=2) | Yes | 
ex4.csv (k=5) | Yes | This file contains two empty sudokus to check how the code performs in worst case (when both sudokus are empty) 
ex5.csv (k=4) | Yes |
ex6.csv (k=3) | Yes | 

5 files have been included for Q2 in the [tests/q2](/Assignment_1/tests/q2/) folder.

Name of the file | Remarks
--- | --- |
k2_1.csv (k=2) | 
k2_2.csv (k=2) | Two files for k=2 are meant to verify the randomness of the generated sudokus.
k3.csv (k=3) | 
k4.csv (k=4) | 
k5.csv (k=5) |

