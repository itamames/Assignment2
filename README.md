# Assignment2

A molecule is made of two or more atoms, where each atom can occur more than once. An atom is represented by an atomic symbol consisting of a single uppercase letter or an uppercase letter followed by a lowercase letter (e.g. H, O, Fl, Na). 

An atom also has an atomic number that represents the number of protons in that atom. For example, the chlorine atom (Cl) has an atomic number of 17, which means it has 17 protons. 

![atoms](Atoms.jpg)

* A molecular formula is a non-empty sequence of atomic symbols (e.g. KBr, CO, LiCl). 
* A molecular formula can consist of a single atom (e.g. H) or a single atom repeated (e.g. O3)

(Extra Credit)
* Part of the formula may be repeated by enclosing it in parentheses followed by an integer between 2 and 99 (e.g. Ca(OH)2). 
* The parentheses are omitted if the repeating component is a single atom (e.g. H2O, C6H12O6, Na2SO4, Ni(NO3)2). 
* It can also consist of multiple levels of parentheses (e.g. Co3(Fe(CN)6)2).

## Assignment

 * Modify the Java program named FormulaCalc.java that has a method that takes a string representing a valid molecular formula and computes and returns the total number of protons in the molecule. Your method should use a stack to keep track of partial results as you encounter subexpression in the chemical formula. 

 * You may assume that the atoms in the formula all have atomic numbers no greater than 54 and appear in the truncated periodic table shown below. Each box shows the atomic symbol along with its atomic number.
 * Use the Java class Stack for your stack class. Do not call any methods except push, pop, empty, and peek.
 * You may assume that if an integer is given in the formula it will be in a valid location and its value will be between 2 and 99, inclusive.
 * You may assume that the given formula is valid, including only atoms shown above and proper layering of parentheses.
 * Your class should also have a main method that tests your formula computation method. See the Testing section for the format for the input and output for testing.

(Extra Credit)

* The program will process parentheses in the formulas.
* The formula can potentially have any number of layers of parentheses.

## Testing

You should write your main method so that it reads input from the keyboard (standard input) and outputs its results to the console (standard output) for testing. The first line of input should be the number of test cases to be executed. Subsequent input will be one chemical formula per line. For each formula, output the number of protons in the formula. Each output should be on a separate line. You do not need any additional prompts or output text.

Or you can use the formulas.txt file in the folder.

Example input:

```txt
H
KBr
H2O
C6H12O6
```

Example output:

```text
1
54
10
96
```


(Extra Credit)

```txt
Ca(OH)2
Ni(NO3)2
Co3(Fe(CN)6)2
```

Example output:

```text
38
90
289
```
