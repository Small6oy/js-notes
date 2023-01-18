# Execution Context

When you run any JS, a special environment is created to handle the transformaiton and execution of the code.
This is call the execution context. It contains the currently running code and everything that aids in its execution

There is global execution as well as a function execution context for every function invoked

## Execution Context Phases

| Memory                            | Execution                         |
|-----------------------------------|-----------------------------------|
|                                   |                                   |
| this is the                       | this is the                       |
| variable env                      | thread of                         |
| that stores                       | execution.                        |
| all of your                       | Each line of                      |
| variables and                     | code is                           |
| functions as                      | executed line                     |
| key value pairs                   | by line                           |
| in memory                         |                                   |
|                                   |                                   |
| eg                                |                                   |
| name: 'Godwin'                    |                                   |
| x: 100                            |                                   |
| y: undefined                      |                                   |
| fn: {}                            |                                   |


### Memory Creation Phase

1. Create the global object (browser = window, Node.js = global)
2. Create the 'this' object and bind it to the global object
3. Setup memory heap for storing variables and function references
4. Store functions and variables in global execution context and set to 'undefined'

### Execution Phase

1. Execute code line by line
2. Create a new execution context for each function call 
