# Test Development and Design
### Objectives
* Understand why we have test design techniques and what a test basis document is used for
* Differentiate between a test design spec, test case spec and a test procedure spec
* Etc.

To Remember: There are no right or wrong ways

Why do we rely on established test design techniques?
* Help us achieve a given level of acceptance and confidence in the software

What would happen if we didn't use these techniques?
* Amount of testing could spiral out of control

## Test Design
You must consider the context (environment) within which the tests are taking place:
* The Organisation
* The maturity of the development and testing process
* Time/resource constraints
* Safety or regulatory requirements
* The people involved

Why is traceability from test procedures back to specifications important?
* It enables both effective impact analysis when requirements change, and determining requirements coverage for a set of tests


* Test Design – The process of transforming general testing objectives into tangible test conditions and test cases.
* Test Base – i.e. Requirements and Specifications
  * Test Approach – implemented to select the test design techniques to use, i.e.:
    * Specification Based/Black Box,
    * Structure Based/Whitebox, Experience/Exploration Based
* Test Plan - A document describing the scope, approach, resources and schedule of intended test activities
  * Test Conditions – An item or event of a system that could be verified by one or more test cases
    * "What needs testing"
    * i.e. Signing into a website would be an test condition, but so could being in a state of ‘Overdrawn’ with a bank account.
  * Test Cases – Information to execute the test i.e. environmental needs, expected outputs
    * "The tests themselves"
    * Test Implementation - The process of developing and prioritising test procedures, creating test data etc.
  * Test Procedures – A robust resource of test scripts to do the testing

### Test Design Specification
* Highest level document we create
* Specifies the test conditions for a test item, the detailed test approach and identifies the associated high level test cases
* Template: **IEEE829**

## Test Cases

Now that we understand the conditions, we can create the Test Cases

These consist of a set of input values:
* Execution Preconditions
* Expected Results
* Execution Post-Conditions

The Objective of compiling the test case specifications is to specify in detail each test case listed in the test design specification

#### Test Case spec example
* Description
* Preconditions
* Steps
* Input
* Expected Result
* Actual Result

### Ways to tackle Test Cases
* Functional
  * Test each function
* Domain
  * Test by partitioning different sets of values
* Specification Based
  * Test against specifications
* Risk Based
  * Imagine a way a program could fail and then design tests to check whether the program will actually fail
* User
  * How the user will approach the system
* Scenario/Use Case
  * Based on actors/users and a set of actions they are likely to perform in real life
* Exploratory
  * The tester actively controls the design of tests as those tests are performed and uses information gained while testing to design new and better tests

### Expected Results
* The most important part of executing tests is knowing why you are doing them in the first place
* If expected results have not been defined, an incorrect result may be interpreted as a correct one

## Test Procedure


## Standardisation
* If a feature has a lot of input combinations, separate the test into subtests
* Write in keeping with standard documentation

## Traceability
* ISTQB Definition
  * Traceability: The ability to identify related items in documentation and software, such as requirements with associated tests
* Ability to trace test conditions to specs and requirements
* Allows impact analysis when the requirements change
* Ensures requirements test coverage can be determined for a set of tests
* Horizontal Traceability: The tracing of requirements for a test level through the layers of test documentation (eg: test plan, test design spec, test case spec & test procedure spec or test script)
* Vertical Traceability: The tracing of requirements through the layers of development documentation to components

## Test Plan
* **IEEE829** Standard
* Master test plan within the IEEE829 document

### Basic Template
1. Test Plan Identifier
2. References
3. Introduction
4. Test Items
5. Software Risk Issues
6. Features to be Tested
7. Features not to be Tested
8. Approach
9. Item Pass/Fail Criteria
10. Suspension Criteria and Resumption Requirements
11. Test Deliverables
12. Remaining Test Tasks
13. Environmental Needs
14. Staffing and Training Needs
15. Responsibilities
16. Schedule
17. Planning Risks and Contingencies
18. Approvals
19. Glossary

## Scheduling
* Once the procedures are complete the test cases can be formed into a test execution schedule
* Defines the order the various test procedures are executed
* Test execution schedule takes into account such factors as regression tests, prioritisation and technical/logical dependencies


* Most important tests must be executed earliest so, even if the time is shortened we have still tested the top priority functionality
* Take into consideration the logical order of execution and technical dependencies
* Highest priority is always run first (possibly taking the opportunity to test any dependencies or relative areas at the same time)
* Regression testing must be done last

Test plans must be highly dynamic due to:
* Changing Priorities
* Defects
* Resources

## Test Coverage
Quantitative measures are extremely important to help stakeholders understand how much of the system has been tested

Need to consider in terms of how much of the system has been tested. EG:
* 2 Weeks of testing - **Bad**
* 80% of the system has been tested - **Good**

Coverage might make up part of the completion criteria defined in the test plan. It can also be used to tell us when to stop testing.
