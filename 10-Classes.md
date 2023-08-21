# Chapter 10: Classes

## Classes should have one responsibility—one reason to change

## Classes should be small

## Classes should be cohesive—cohesion results in many small classes
Classes should have a small number of instance variables. The more variables a method manipulates the more cohesive that method is to its class. Try to separate the variables and methods into many small classes such that the classes are more cohesive.

## Follow the Law of Demeter
The Law of Demeter says that a method f of a class C should only call the methods of these:
- C
- An object created by f
- An object held in an instance variable of C
- An object passed as an argument to f

TODO [Provide example of the Law of Demeter]
`
export class Cocktail extends xxx {
    constructor() {}

    getABV() {

    }

    getIngredients(): {
        
    }
}
`

## Use data abstraction
Abstraction gives the freedom to change implementation.

## Incorporate new features by extending the class
Incorporate new features by extending the class, not by making modifications to existing class, to reduce the risk of change.

## Treat the Active Record as a data structure
Create separate objects that contain the business rules. Data structures expose their data. Objects expose functions that operate on data.