# Chapter 5: Formatting

- Use vertical separation for separate concepts
  - Each blank line is a visual cue that identifies a new and separate concept.
- Use vertical density for tightly related concepts
  - Lines of code that are tightly related should appear vertically dense.
- Place dependent functions vertically close
  - If one function calls another, they should be vertically close, and the caller should be above the callee.
- Place similar functions vertically close
  - If a group of functions perform a similar operation, they should be vertically close.
- Declare variables vertically close to their usage
- Horizontal Formatting
  - You should leverage a linter to set a maximum width to your lines of code, maintaining legibility is key.
- Consistent Indentation
  - Leverage the use of a linter to indent on saving the file to prevent inconsistent spacing and reading pace.


## Summary
The use of a linter for your system's code does a number of things for your codebase and your team. The best thing about this chapter is that almost all of it can be automated. The team can sit together to decide on the rules to implement, these are encoded and enforced on save. This saves effort on reviewing code and onboarding new members. These rules you agree upon with your team will not necessarilly be what you personally think is best, but will be what you all decide on together as a team.

## Homework
Implement a linter in a project to do that following
- Set Maximum width on lines of code
- Automatically space out variable and operators
- etc etc TODO Fill in more tasks