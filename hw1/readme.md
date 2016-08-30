# Homework 1, K-State CIS 301, Fall 2016

* **Deadline:** Wednesday, September 7, 2016, 11:59pm US Central 

* **Total Points:** 20

## Assignment Purpose 

- Learn the syntax of propositional logic formulas

- Determine the meaning (determine the truth value) of a 
  propositional logic formula using truth tables

- Understand the correspondence between proposition logic
  formulas and circuits

## More Conventions

* For all the problems below, we use small letters ``p``, ``q``, 
  ``r``, and ``s`` to represent propositional claims.
  In your solutions, please use small letters and preserve
  the letter ordering.
  That is, in a truth table, we assume alphabetical ordering on 
  the inputs, e.g., ``q`` after ``p``) and no substitutions
  (e.g., replacing ``p`` with ``q``, and vice versa).
  For gates with two inputs such as the *and* gate below:

  ![and](and.png)

  The first input should be written on the left-hand side and
  the second input should be written on the right-hand side,
  i.e., ``p ∧ q`` instead of ``q ∧ p`` even though *and* is
  [commutative](https://en.wikipedia.org/wiki/Commutative_property).
  Any deviation of the above conventions results in point deductions.

* On the other hand, you can use either the ASCII or the Unicode
  symbols for the operators *and* (``∧``, or ``^``), 
  *inclusive-or* (``∨``, or ``V``), *negation* (``¬``, or ``~``),
  and *implication* (``→``, or ``->``); the
  Logika IntelliJ (LIVE) plugin features
  [Key Shortcuts](http://logika.sireum.org/doc/02-live/index.html#shortcuts)
  for inserting Logika Unicode operators.
  Note that if you use Unicode, it is best to use 
  [fixed-width font (even for Unicode characters)](http://logika.sireum.org/doc/02-live/index.html#using-a-fixed-width-font)
  when editing your solutions. 
  
The above conventions are applicable for subsequent assignments. 

## Problem Descriptions

1. [3 points]
   It is often useful to have the *exclusive-or* operator/gate;
   given two inputs ``p`` and ``q``, it produces ``T`` if 
   ``p`` and ``q`` are not equal.
   This behavior can be described using *and*, *inclusive-or*,
   and *negation* operators/gates as follows:
   ``(p ∨ q) ∧ ¬(p ∧ q)``. 
   Give a Logika truth table to prove this claim.

2. [3 points]
   Equality of two inputs ``p`` and ``q`` can be expressed
   using *implication* and *and* operators as follows:
   ``(p → q) ∧ (q → p)``.
   Give a Logika truth table to prove this claim.

3. [5 points]
   Give a corresponding Logika truth table for the circuit below:
   
   ![circuit](3.png)
   
4. [9 points]
   By now, you have seen truth tables with up to three input
   variables; to further
   [grok](https://en.wikipedia.org/wiki/Grok#In_computer_programmer_culture)
   the scaling behavior in complexity with reasoning about formula
   with larger inputs, give a Logika truth table for the following
   proposition with four input variables:
   ``¬(p ∨ s) ∧ (q ∨ ¬r) → r → q``.
   