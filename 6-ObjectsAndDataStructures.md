# Chapter 6: Objects and Data Structures

- Hide internal structure.
- Prefer data structures.
- Avoid hybrids structures (half object and half data).
- Should be small.
- Do one thing.
- Small number of instance variables.
- Base class should know nothing about their derivatives.
- Better to have many functions than to pass some code into a function to select a behavior.
- Prefer non-static methods to static methods.

## Summary
Objects expose behaviour and hide data. This makes it easy to add new kinds of objects without changing existing behaviours. It also makes it hard to add new behaviours to existing objects.

Data Structures expose data and have no significant behaviour. This makes it easy to add new behaviours to existing data structures but makes it hard to add new data structures to existing functions.

In any given system we will sometimes want the flexibility to add new data types, and so we prefer objects for that part of the system. Other times we will want the flexibility to add new behaviours, so in that part of the system we prefer data types and procedures. It is important to try to identify these opportunities without prejudice for the job at hand.