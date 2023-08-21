# Chapter 1: Clean Code

## The Total Cost of Owning a Mess
Over a number of years a project can become increasingly complex, small changes begin to take longer and longer and the team's velocity aproaches 0. More knots and tangles are added, new joiners don't have the context of the project so each change could thrawrt the design of the system.

## The Grand Redesign in the Sky
Once the team finall rebels, insisting they cannot continue to work in the current system, management agrees, creates a new team to lead the redesign which is now in a race with the existing team to rebuild what is there, but also to keep up with the new features. This can become a protracted project that goes on for years, and by the time it's complete the original redesign team have all moved on. The redesign then falls into disarray.

Maintaining your existing codebase well using agreed upon standards is the best thing for your project and career.

## the Boy Scout Rule
Leave the camp ground cleaner than you found it.

## Prequel and Principles
- Single Responsibility Principle (SRP)
- Open Closed Principle (OCP)
- Dependency Inversion Principle (DIP)


## What is Clean Code
> Clean code is simple and direct. Clean code reads like a well-written prose. Clean Code never obscures the designer's intent but rather is full of crisp abstractions and straightforward lines of control. ~ Grady Booch

> Clean code can be read and enhanced by a developer other than it's original author. It has unit and acceptance tests. It has meaningful names. It provides one way rather than many ways for doing one thing. It has minimal dependancies, which are explicitly defined, and provides a clear and minimal API. Code should be literate since depending on the language, not all necessary information can be expressed clearly in code alone. ~ "Big" Dave Thomas

> I like my code to be elegant and efficient. The logic should be straightforward to make it hard for bugs to hide, the dependencies minimal to ease maintenance, error handling complete according to the articulated strategy, and performance close to optimal so as not to tempt people to make the code messy with unprincipled optimizations. Clean code does one thing well. ~ Bjarne Stroustrup [Inventor of C++]

> Runs all the tests, Contains no duplication, expresses all the design ideas that are in the system, Minimises the number of entities such as classes, methods, functions and the like. ~ Ron Jefferies [C# Author "Extreme Programming" books]