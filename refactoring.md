# Functional Programming

It is a programming paradigm - a style of building the structure and elements of computer programs - that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

  * Pure functions: It returns the same result if given the same arguments (it is also referred as deterministic) and   it does not cause any observable side effects
  * If a function takes in global or reading files, rng, or makes side effects, it is NOT pure
  * Pure wants functions to be isolated and unable to impact other parts of the system
  * Pure functions are stable, consistent, and predictable. Given the same parameters, pure functions will always   return the same result
  * It needs immutability, when data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

## Functions as first-class entities

The idea of functions as first-class entities is that functions are also treated as values and used as data. Functions as first-class entities can:

   * refer to it from constants and variables
    
   * pass it as a parameter to other functions
   
   * return it as result from other functions

## Higher-order functions

   * When we talk about higher-order functions, we mean a function that either takes one or more functions as arguments, or returns a function as its result

