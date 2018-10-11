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

## Estimation
### Test Planning Activities
* Scope and Risk
* What to test
* Who will test what
* Scheduling
* Levels of detail
* Test Levels and entry/exit criteria

### Methods of Estimation
* Metric Based
  * Relies on Data collected from previous or similar projects
  * Fairly accurate when comparing similarly sized projects
* Expert Based
  * Estimations are based on experience
  * Could be from:
    * Developers
    * Analysts
    * SMEs
    * Test Consultants
    * etc.
  * It can be similar to the Wideband Delphi approach, but not always done in that exact way (Not part of exam)

### Test Progress Monitoring and Control
* Based on activities and timescales within the Test Plan
* Need to constantly review actual against planned
  * Provides important visibility of project progress
* The information is also important to measure test coverage and determine if we have reached the exit criteria goal

### Common Metrics
* Percentage of work done
* Number of test cases executed
* Defect totals and details
* Subjective confidence of release
* Milestones achieved

Metrics should be gathered during and at the end of a test level

### Test Reporting
Reporting test status is about effectively communicating our findings to other project stakeholders

Reporting should include (according to IEEE-829):
* Test Summary Report Identifier
* Summary
* Variances
* Comprehensive Assessment
* Summary of Results
* Evaluation
* Summary of Activities
* Approvals

### Test Control
By monitoring the progress of the project, we are allowing outselves to take corrective measures to ensure we stay on target

Activities Include:
* Re-prioritising tests
* Change the test schedule
* Review product risks
* Adjust the scope

## Configuration Management
Core Parts:
* Configuration Identification
  * Identification of Docs, Labelling Hardware, Grouping of related items
* Control
  * All changes to a complex system are performed with the knowledge and consent of the managements
* Status Accounting
  * Provides the means by which the current state of development can be judged and history of the life cycle can be traced
* Auditing
  * Confirms the integrity of a systems product prior to delivery
  * Two types:
    * Function
    * Physical

### Dangers if not handled correctly
* Multiple people working on the same element at the same time without any knowledge of the others' work
* Not able to match program source to object code
* System being difficult to maintain as the documents are not correct

### Other Benefits
Allows for the Identification and reproduction of:
* Test Items
* Test Documents
* Tests
* Test Harness

## Risk
Two types of risk:
* Product Risk
  * Factors related to what is produced by the work, IE: What is being tested
* Project Risk
  * Factors relating to the way the work is carried out, IE: The test project

### ISTQB Definitions
Risk
* A factor that could result in future negative consequences
  * Usually expressed as impact and likelihood

Risk Analysis
* The process of assessing identified risks to estimate their impact and probability of occurrence

### Product Risk
* Failure Prone Software
* Potential for the software/hardware to cause harm
* Poor software characteristics, EG:
  * Security
  * Reliability
  * Maintainability
  * Performance
* Poor data integrity/quality

### Project Risk
* Failure of a third party
* Contractual Issues
* Skills, Training and Staff shortages
* Personal Issues
* Political Issues
* Improper Attitude
* Defining the right requirements
* Time and Budget
* Environment inadequacy
* Low Quality of data

### Quantifying Risk
Use of the Risk Matrix

* Likelihood
* Impact

### Risk-Based Testing
* Designed to reduce the level of product risks and inform stakeholders of their status
* Involved the identification of product risks and the use of risk levels to guide test process
  * Make prioritised list of risks
  * Perform testing that explores each risk
  * As risks evaporate and new ones emerge, adjust to stay focused on the risks at the time

## Incident Management
Process of recognising, investigating, taking action and disposing of incidents

Involves:
* Logging incidents
* Classifying them
* Identifying the impact

### Incident Reports (Defect Reports)
* Can be raised at any time by anyone
* Whoever discovers the problem writes it (Usually the Testers)

Core Objectives:
* Provide as much info on the problem as possible
* Allow incident to be tracked and easily reported on, helping to supply metrics
* Help develop test improvements, identify how the functionality should be tested next time

#### Typical Content
* Date, time, who, where, status
* Scope, Severity, Priority
* Urgency
* References
* Expected to actual results
* High level description of the incident
* Detailed description of the incident
* Conclusion
