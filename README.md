Dean Yu

This repo is a clone of https://github.com/mjhea0/flaskr-tdd.

# Add Test Cases to Group Project

Unit Tests:
- test_degree.py: 
	- https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/lab6/dean/Education_Pathways/tests/test_degree.py#L1-L94
	- https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/lab6/dean/Education_Pathways/tests/test_degree.py#L179-L268
	- https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/lab6/dean/Education_Pathways/tests/test_degree.py#L341-L385
- test_student.py: 
	- https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/lab6/dean/Education_Pathways/tests/test_student.py#L1-L172

Integration Tests:
- test_sv_api.py:
	- https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/lab6/dean/Education_Pathways/tests/test_sv_api.py#L1-L269

Frontend Tests:
- test_sv_frontend.py:
	- https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/lab6/dean/Education_Pathways/tests/test_sv_frontend.py#L1-L200
- test_mc_frontend.py:
	- https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/lab6/dean/Education_Pathways/tests/test_mc_frontend.py#L1-L124
- test_course_frontend.py:
	- https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/lab6/dean/Education_Pathways/tests/test_course_frontend.py#L1-L35

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
