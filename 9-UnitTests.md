# Unit Tests
> Test code should be maintained to the same standards of quality as their production code.
## 3 Laws of TDD

1. You may not write production code untill you have written a failing unit test.
2. You may not write more of a unit test than is sufficient to fail, and not compiling is failing.
3. You may not write more production code than is sufficient to pass the currently failing test.

## Unit Test Guidelines
- One Assert per Test
- Single Concept per test
  - Don't merge multiple things into one test. It may confuse the next developer to read it. This would also require multiple Asserts.

## F.I.R.S.T

**Fast**: Tests should be fast. They should run quickly. When tests run slow, you won’t want to run them frequently.

**Independent**: Tests should not depend on each other. One test should not setup the conditions for another test. Each test should be able to be run independently, in any order.

**Repeatable**: Tests should be repeatable in any environment, at any time. You should be able to run your tests from Local, to QA, to Production.

**Self-Validating**: Tests should have a boolean output. Either they pass or fail. You should not have to read through logs, nor compare between text files to determine if it passed or not. That would lead to test results becoming subjective, which they should never be for code.

**Timely**: The tests need to be written in a timely fashion. Unit tests should be written just before the production code that makes them pass. If you write tests after the production code, then you may find the production code to be hard to test. This is the very code that should be tested or refactored, as it has not been designed to be tesed.