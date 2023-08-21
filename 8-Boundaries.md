# Chapter 8: Boundaries
The boundaries between our code, and 3rd party code, be it from another Business Unit or library, should be clear and concise. We do this by using as little of their code in ours as is possible. 

# Learning Tests
Learning tests are free and have a positive return on investment. Learning Tests are precise experiments that helped increase our understanding of the package we are importing. Learning tests verify that the 3rd party packages work the way we expect them to. If a version update to that package breaks our compatibility, we will find out right away. 

# Defining a Boundary
If you are importing a library for a required piece of functionality, like a Table/Table package, instead of importing the package's main class directly into your code, you can always abstract that out by defining your our class that is actually imported throughout the application, and this class will extend the class from the package. This way if your requirements change and a rework is underway, your codebase isn't cluttered with 3rd party classes.

e.g. 
`export class AnPoitigeirTable extends AGGridTable {}`

## Summary
We manage 3rd party boundaries by referring directly to them infrequently. We wrap them, or we write an Adapter for them, to adjust the interface we require, and taking controll of the boundary.