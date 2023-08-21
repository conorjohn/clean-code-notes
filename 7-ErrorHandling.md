# Chapter 7: Error Handling

- Put all code inside try block
  - If the keyword try exists in a function, it should be the very first word in the function and there should be nothing after the catch/finally blocks.
- Prefer exceptions to returning error codes
  - Returning error codes leads to deeply nested structures. If you use exceptions instead of returned error codes, then the error processing code can be separated from the happy path code.
- Use wrapping to return a common exception type
  - We can simplify our code considerably by wrapping the API that we are calling and making sure that it returns a common exception type.
  - Find a Node/JS/Angular equivelant to the example here: https://erik-uus.gitbook.io/clean-code/key-principles/error-handling 
- Define Exception Classes in Terms of the Caller's Needs
- Don't return null

## Summary
Clean code is readable and robust. The purpose of Error Handling is to leave your application in a consistent state. We can write robust clean code if we see error handling as a separate concern, viewable independently from our main logic. Reasoning about and defining our error handling independently of our logic massively improves the maintainability of our code.