# Refactoring 

---


### Functional programming 
- a programming paradigm a style of building the structure and elements of computer programs

    Pure functions 

    It returns the same result if given the same arguments (it is also referred as deterministic)
    It does not cause any observable side effects
    Pure functions benefits
    easier to test codes
- impure functions 

    with global var
    readings external files
    random number generator

- Immutability 

    Unchanging over time or unable to be changed.
- referential transparency 

    pure functions + immutable data = referential transparency
- Functions as first-class entities  CAN:

    refer to it from constants and variables
    pass it as a parameter to other functions
    return it as result from other functions

- Higher-order functions 

    takes one or more functions as arguments, or
    returns a function as its result
### Refactoring JavaScript for Performance and Readability 

*Strategies There are no absolutes when it comes to clean code — there's always an edge case!*
- Return early from functions
- Cache variables so functions can be read like sentences
- Check for Web APIs before implementing your own functionality