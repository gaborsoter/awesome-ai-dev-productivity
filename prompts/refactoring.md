# Refactoring Prompt


## Breaking up complex code
_model_ : GPT-4

Given the complex code or function provided, please refactor it in adherence to the following best practices:

1. **Single Responsibility Principle**: Break down the code such that each function/method does one thing and does it well. This will make the functions easier to test and understand.
2. **Descriptive Naming**: Rename variables, functions, and classes to be self-explanatory, indicating their purpose or usage. Avoid acronyms and abbreviations unless they are universally recognized.
3. **Use Comments Sparingly**: Aim for the code to be self-documenting through clear structure and naming. However, if there's a particularly complex algorithm or workaround, document it briefly with a comment.
4. **Eliminate Global Variables**: If the code uses global variables, try to pass them as parameters or encapsulate them within classes or structures to avoid unintended side effects.
5. **Abstract External Dependencies**: If the code interacts with external systems, databases, or third-party services, abstract these dependencies. This will allow for easier mocking during testing and will decouple the code from specific external implementations.
6. **Limit Nesting**: Reduce deep nesting by using guard clauses or breaking up the logic into smaller functions.
7. **Error Handling**: Ensure errors or exceptions are handled gracefully. If exceptions are thrown, they should be specific to the error and provide clear messages. Consider using a unified error handling mechanism.
8. **Use Data Structures Efficiently**: If the code uses data structures, ensure that they are used efficiently and are appropriate for the task. For example, avoid using lists where a set or dictionary might be more efficient.
9. **Minimize Side Effects**: Functions should preferably be pure, meaning they do not modify external state and for the same input always produce the same output.
10. **Use Parameterized Functions**: Rather than hardcoding values, allow functions to be more flexible by passing parameters.
11. **Automated Formatting**: Ensure consistent formatting across the refactored code, making use of automated tools if necessary for uniformity.