# Chapter 17: Smells and Heuristics

## Intro
This list of code smells can help a developer going through a Pull Request, the details help a developer identify issues that may develop beyond the initial "looks like it works to me" scan. These are signs and principals that a Senior can point out to a more Junior developer to help them improve their own code.

## Comments
- Inappropriate Information
- Obsolete Comment
- Redundant Comment
- Poorly Written Comment
  - Use correct Grammer and punctuation, don't ramble
- Commented-Out Code

## Environment
- Build requires more than One Step
- Tests Require more than One Step

## Functions
- Too Many Arguements
- Output Arguements being Counter Intuitive
- Flag Arguments
  - Boolean arguments loudly declare that a function does more than one thing. This leads to confusion and should be eliminated
- Dead Function
  - Remove any method that is never called.

## General
- Multiple languages in 1 Source File
- Obvious Behaviour is unimplemented
  - If a method doesn't work in the expected manner, trust can be broken in the original author.
- Incorrect Behaviour at the Boundaries
- Overridden Safties
  - Warnings and Tests are in place for a reason, do not disable them for a quick win.
- Duplication
- Code at the wrong level of Abstraction
- Base Classes Depending on Their Derivataives
- Too Much Information
- Dead Code
- Vertical Separation
- Inconsistency
- Clutter
- Artificial Coupling
- Feature Envy
- Selector Arguments
- Obscured Intent
- Misplaced Responsibility
- Inappropriate Static
- Use Explanitory Variables
- Function Names should Say What They Do
- Understand the Algorithm
- Prefer Polymorphism to If/Else or Switch/Case
- Follow Standard Conventions
- Replace Magic Numbers & Strings with Named Constants
- Encapsulate Conditionals
  - try not to have a chained list of conditions in one if statement
- Avoid Negative Conditionals
- Functions should do one thing.
  - Only contain one loop, if or calculation before passing the result to the next method

## Java/Type(Script)
### Wildcard Imports
- Some packages are quite large, and because our applications need to be downloaded by a browser, we should be keeping our bundles as small as possible.
- 
### Constants vs Enums
- Now that ENUMs are available, USE THEM! The meaning of a const may not be clear, where as an ENUM is unmistakeable.

## Tests
- Insuffient Tests
- Use a Coverage Tool
- Don't Skip Trivial Tests
- An Ignored Test Is a Question about an Ambiguity
- Test Boundaray Conditions
- Exhaustively test near bugs (Bugs tend to congregate)
- Patterns of failure are revealing
- Tests should be fast

# Summary
This list is not exhaustive, but should be looked at as initial guide lines that you can revise and edit based on your own project and codebase.

## Homework
Implement a Code Smell tool like Sonar.