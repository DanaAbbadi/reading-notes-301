# Call stack

It’s a mechanism for an interpreter to keep track of its place in a script that calls multiple functions: specifically, what function is currently being run and what functions are called from within that function, etc
When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.

When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
If the stack takes up more space than it had assigned to it, it results in a “stack overflow” error.

# JS Call Stack

The JavaScript engine is a single-threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.

The call stack is primarily used for function invocation. Since the call stack is single, function execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

asynchronous js has a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.
call stack is a data structure that uses the Last In, First Out principle to temporarily store and manage function invocation (call).

When a function is invoked, the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.

Manage function invocation (call): The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error


### JavaScript error messages && debugging

The first thing that indicates you that something is wrong with your code is the (in)famous error message that the one we saw just moments ago, it usually appears on your console (being developer tools of the browser, terminal or whatever else you are using).

Types of error messages:

  * Reference errors
  * Syntax errors
  * Range errors
  * Type errors

# Debugging

To debug your JS code, the easiest and maybe the most common way its to simply console.log() the variables you want to check or, by using chrome developer tools, open your page with your JS code (press cmd+o in macOS or Ctrl+o in Windows) and choose your file to debug, click the line you wanna debug and refresh your page again (F5).

### Tools to avoid runtime errors

* quokka
* eslint