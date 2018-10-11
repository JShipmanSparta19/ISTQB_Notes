# Test Management
### Objectives
* Recognise the different roles in a test team and the associated tasks
* Understand the importance, benefits and drawbacks of independent testing within an organisation
* Recognise key test planning activities and objectives
* Differentiate between two conceptually different estimation approaches
  * the metrics based approach
  * the expert based approach
* Recall common metrics used for monitoring test preparation, execution, reporting and control
* Summarise the purpose and content of the test summary report document according to IEEE-829
* Differentiate between conceptually different test approaches, such as analytical model based methodical, process/standard compliant, dynamic/heuristic, consultative and regression averse
* Summarise how configuration management supports testing
* Define the term "risk" and understand that risks are determined by likelihood and impact
* Distinguish between the project and product risks, explaining with examples, how risk analysis and risk management may be used for test planning
* Recognise and contextually apply the content of an incident report according to the Standard for Software est Documentation (IEEE-829-1998)

## Organisation
Roles within a Project:
* Project Managers
* QA Managers
* Developers
* Business and Domain Experts (SME, Business Analyst)
* Infrastructure Personnel (Database Designers, etc.)
* IT Operations (Help desk, merge functionality, etc.)

### Test Leaders
* Project Manager
* QA Manager
* Development Manager
* Manager of test group

#### Typical Tasks for a Test Leader
* Co-ordinate and possibly write and review test strategy (for the project) or policy (for the organisation)
* Plan and negotiate with project managers and other stakeholders
* Directs spec, prep, implementation and execution of tests
* Time, effort and cost
* Report - Progress Vs Actual
* Quality of the work product and the quality of the testing
* Ensures the appropriate training has taken place
* Make sure the appropriate environments are in place

### Tester
* Developers
* Business Analysts
* Users
* SMEs
* Specialists

#### Typical Tasks for a Tester
* Review and contribute to the test plans
* Review Requirements
* Test Specification and Test Cases based on the techniques given in the Test Plan
* Prepare Test Data
* Execute test procedures, log, evaluate results and document any deviation
* Use test admin, management and monitoring tools
* Automate Tests (possibly supported by a developer or automation expert)
* Review Tests developed by others

### Key Differences between Test Leaders and Testers
* Test Leader: Manages the tests
* Tester: Performs the tests

## Independence
* "Separation of Responsibilities, which encourages the accomplishment of objective testing"
* Effectiveness of finding defects by testing and reviews can be improved by using independent testers. It is thought that the software is tested more thoroughly
* Extremely powerful in situations where an independent tester is used to test, rather than the author of a work product

### Testing Independence Levels Within an Organisation
1. No Independent Testers
  * Developers test their own code
2. Independent Testers within the development team
3. Independent test team or group within the organisation
4. Independent Testers from the Business or User Community
5. Independent Test Specialists in usability, security, etc.
6. Independent Testers external to the organisation


* It is possible that they may be responsible for defining test features and rules

#### Benefits Vs Drawbacks
Benefits:
* See defects that others who are closer to the project may not
  * They should be unbiased
* Can verify assumptions made during the specification and implementation phases

Drawbacks:
* Can be seen as not part of the project and suffer from isolation
* Can be easily blamed for delays and targeted as delivery bottlenecks
* Developers may no longer feel responsible for their mistakes
* High Costs
