Dean Yu

This repo is a clone of https://github.com/mjhea0/flaskr-tdd.

# Pros and Cons of TDD

Pros:

- No redundant code
    - Since only the necessary code to pass the given test cases is written, there should be little or no redundant code
- Code should have good coverage of edge-cases
	- Since the test cases are the focal point of this style of development, significant time is spent trying to cover all edge-cases in the test cases.
    - Thus, the code produced should have a high level of robustness

Cons:

- Limits the potential for high level architecture design
	- Since you are only implementing the bare minimum that you need for a given test case, you don’t really have an opportunity to think ahead and consider how various components should interact
	- Although architecture design can be improved in the refactor phase, this approach is more time consuming then directly implementing the most appropriate architecture
- Some components are difficult to create tests for before they are implemented
	- Frontend tests are difficult to create before implementing the frontend since you don’t know the component names and page layouts beforehand
- Some tests cannot be automated
	- Such tests require manual testing
	- For example: how visually appealing a css style looks
