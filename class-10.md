# The Call Stack and Debugging

---

### call stack
- a mechanism 🔩 for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions

    When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
    Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
    When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
    If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

### Understanding the JavaScript call stack 
- The JavaScript engine  (which is found in a hosting environment like the browser), is a single-threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.

`call stack_ is a data structure that uses the _Last In, First Out (LIFO)_ principle to temporarily store and manage function invocation (call)`

 - The key takeaways from the call stack are:

    It is single-threaded. Meaning it can only do one thing at a time.
    Code execution is synchronous.
    A function invocation creates a stack frame that occupies a temporary memory.
    It works as a LIFO — Last In, First Out data structure.
    JavaScript error messages && debugging 
    Types of error messages

    Reference errors: use a variable that is not yet declared
    Syntax errors: something that cannot be parsed in terms of syntax
    Range errors: manipulate an object with some kind of length and give it an invalid length
    Type errors: undefined type of variable
    Debugging 

    Using Node.js with Visual Studio Code
    Tools to avoid runtime errors 

    quokka to evaluate your code as you type
    eslint to make sure your style guide is consistency and it will grab you an error or two along the way and
    to make JS a more strong typed experience you can check out stuff like TypeScript.