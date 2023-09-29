# Unit tests prompts

## Core Unit test
_model_ : GPT-4

Given the function or code snippet provided, please generate unit tests that adhere to the following guidelines:

1. **Coverage**: Ensure that every line, branch, and edge case of the function/code is covered by the tests. This includes happy paths, edge cases, and potential error scenarios.
2. **Isolation**: Each test should verify one specific behavior or aspect of the function. If a test fails, it should be clear which specific part of the function is malfunctioning.
3. **Descriptive Test Names**: Each test name should clearly describe what it's testing. Use the format: **`test_<functionName>_<conditionOrScenario>`**.
4. **Arrange-Act-Assert**: Structure each test using the Arrange-Act-Assert (AAA) pattern.
    - **Arrange**: Set up the data and environment for the test.
    - **Act**: Call the function with the set up data.
    - **Assert**: Verify the function returned the expected result or threw the expected exception.
5. **Use Mocks and Stubs**: If the function interacts with external systems, databases, or third-party services, use mocks and stubs to simulate those interactions to ensure that the tests only validate the functionality of the function itself.
6. **Parameterized Testing**: Where applicable, use parameterized tests to run the same test logic with different input values.
7. **Document Assumptions**: If any assumptions are made about the context in which the function operates, or the data it processes, document these in the test as comments.
8. **Cleanup**: If a test creates any data or alters any state, ensure it's cleaned up after the test runs, ensuring no side effects.

Using the above guidelines, please generate unit tests for the following function/code: