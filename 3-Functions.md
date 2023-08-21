# Chapter 3: Functions

Functions should
- Be Small
- Do One Thing
- Follow the stepdown rule
  - We want every function to be followed by those at the next level of abstraction so that we can read code from top to bottom.
    - `function pay(value: number)`
    - `function payIfNecessary(employee: Employee)`
    - `function calculateAndDeliverPay(employee: Employee)`
- Avoid nested structures
- Use descriptive names
- Use few arguments
  - The ideal number of arguments for a function is zero. Three arguments should be avoided where possible.
- Avoid flag arguments
  - Function with flag argument does more than one thing. It does one thing if the flag is true and another if the flag is false!
- Have No Side Effects
  - Functional programming paradign should be followed as close as is reasonable. 
- Separate command from query
  - Functions should either do something or answer something, but not both.
- Prefer exceptions to returning error codes
  - Returning error codes from command functions leads to deeply nested structures. If you use exceptions instead of returned error codes, then the error processing code can be separated from the happy path code.
- Put all code inside try block
  - If the keyword try exists in a function, it should be the very first word in the function and there should be nothing after the catch/finally blocks.

## Summary
Functions are the Verbs of your language of choice, Classes are the Nouns. Consider telling a story about what each page of your app does and you should find yourself actually using the names you have used for Classes and Functions.