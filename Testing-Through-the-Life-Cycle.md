# Testing through the Lifecycle
### Objectives
* Explain Relationship between development test activities and work products in the SDLC
* Etc.

## Fundamental Test Process
1. Test Planning and Control
2. Test Analysis and Design
  * Can return to 1.
3. Test Implementation and Execution
  * Can return to 2.
4. Evaluating Exit Criteria and Reporting
  * Can return to 2.
5. Test Closure Activities

### Test Planning and Control
* Determines what is going to be tested
* How is it going to be tested
* Who is doing the testing
* How it will be achieved
* Will also **determine exit criteria**
  * Exit Criteria - What needs to be achieved before the testers can leave
  * Think about Decision/Statement Coverage (Not that common)

### Test Analysis and Design
* The fine detail of what to test
* Test conditions, cases and procedures
  * Conditions - A characteristic of our software that we can check with a test or set of tests.
  * Cases - The actual tests we're going to be doing - Gets to a start point (Execution Preconditions), Input values to achieve an expected result, leaves the system at an end point (Execution post conditions)
  * Procedures - The methodology for the tests (script)
* **The Test Base is reviewed**
  * Body of knowledge used as the basis for test analysis and design
* We look at how to combine test conditions into test cases

### Test Implementation and Execution
* Most visible part of testing
* Prioritising test cases
* Creating test suites from collected test cases
  * A set of test cases or test procedures to be executed in a specific test cycle
* Environment set-up
* Log testing activities and defects
  * Write up results in a log (EG: JIRA)
* Running tests

### Evaluating Exit Criteria and Reporting
* Has the criteria been met to satisfy the stakeholders?
* Does the system do as expected?
* Determine if more tests need to be made
* Is the system ready for release?

### Test Closure Activities
* Make sure docs are up to date and archived
* Passing over testware to maintenance teams if available
  * Enable Support staff to test the software and resolve issues
* Lessons learnt

## Development Models
Methodology chosen depends on the:
* Nature of the project
* Project schedule
* Resource availability

### **Waterfall**

### ***V-Model***
* Requirement Spec
  * -> Planning -> Acceptance Testing
  * Capturing of user needs
* Functional Spec
  * -> Planning -> System Testing
  * Definitions of functions required to meet user needs
* Tech Spec
  * -> Planning -> Integration Testing
  * Technical design of functions identified in Functional Spec
* Program Spec
  * -> Planning -> Unit Testing
  * Detailed design of each module or unit to be built to meet required functionality
* Coding
* Unit Testing
* Integration Testing
* System Testing
* Acceptance Testing


* Validation - Check if docs are current, no information lost, no ambiguities/errors
* Verification - Check if docs still satisfy the original requirements

Pros:
* Test plans developed earlier
* Defects found earlier


* Integrates testing into the whole dev process
* At each
* Can have extra levels of testing, EG: System Integration testing between System and Acceptance

### **Incremental (Agile)**
