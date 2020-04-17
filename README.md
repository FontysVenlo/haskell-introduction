---
title: "PPAR Course  - Haskell Introduction"
author: [Stefan Sobek]
date: "2020-04-15"
subject: "Haskell"
keywords: [Fontys, Haskell]
lang: "en"
titlepage: "true"
logo: "images/fontyslogo.png"
titlepage-rule-color: "400070"
...

# Haskell introduction

This Haskell Workshop is currently part of a course called PPAR - Programming Paradigms of Fontys University of Applied Sciences and is based on the the haskell workshop from two students who prepared it for the ESD - course in Informatics study programme at Fontys Venlo in 2018. Thank you very much [Marco Kull](https://github.com/MarcoKull) and [Jan Evers](https://github.com/Backend-Giraffe). 

## Purpose

The purpose of this workshop as part of the PPAR course is to give a brief introduction of Haskell. 

### The main learning goals

- Get familiar with Haskell language and the compiler
- Know what this functional programming language is and what the benefits of using it are

## Principles of functional programming

> Functional programming is a programming paradigm a style of building the structure and elements of computer programs that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 
> Wikipedia

![Haskell vs OO](images/haskell-intro.png)

### Pure functions
- Returns same result if given same arguments, also referred as deterministic.
- It does not cause any observable side effects.  
- What is then an impure function??? 
    - Imagine a java class with a field, where the field will be used in a calculation. This field was not passed as parameter to the function! The java class has a state which could have influence on the method.
   
### No side-effects

- No change of reference variables
- e.g. in Java, passed by reference parameters!!! If you change the value of the passed parameter, you change the whole reference variable. 

### Immutability
- „unchanging over time or Unable to change“

## What is a function?

- Function has inputs and an output 

![Inputs and Outputs](images/input-output1.png)

- Output (result) depends on the inputs (parameters)
- Simple example: 

![Simple example](images/input-output2.png)

- Another example: 

![Input and Output other example](images/input-output3.png)

## What is Haskell?

- Purely functional programming language 
- You tell the computer what stuff is, rather than what to do (declarative style) 
- Features: 
    - Type inference 
    - Statically typed 
    - Lazy evaluation 
    - ...
    
![images/lazy-when-smart.png](images/lazy-when-smart.png)

## To infinity and beyond

![images/inifinity1.png](images/inifinity1.png)

// TODO: infinite loop example

## Where are my loops?

- Remember: imperative vs. declarative style 
- But how do I work with lists then? 
    - MAP
        - Transform elements in a list
    - FOLD (left, right)
        - Reduce list to one value
    - ZIP (with)
        - Combine elements from two lists
    - FILTER
        - Well... removing some elements
- Do you remember lambda calculus?

// TODO: map example

## Pure functions in Haskell

- All functions take a parameter 
- All functions must return a value 
- Anytime a function is called with the same parameter it returns the same value 
    - *Output depends ONLY on parameters*

