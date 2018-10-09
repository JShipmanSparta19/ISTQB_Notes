# ISTQB Preparation Notes

1. **Fundamentals of Testing**
2. **Testing through the Life Cycle**
3. **Testing Levels**
4. **Static Testing Techniques**
5. **Test Development and Design**
6. **Testing Techniques**
7. **Test Management**
8. **Tool Support for Testing**
9. **Defect Management**

#### Core Objectives
* Need to understand why we do testing.
* Effects of a software defect, distinguish between root cause and effect.
* Etc.

#### Intro
* Why do we need testing?
  * Making sure it's up to quality standards.
* How might testing contribute to better quality software?
  * Ensure that all requirements have been met.
* What is quality?

#### Exams
* 40 Questions, 26 to pass
  * Need to get 30 in 2 mocks to do the exam
* K-Levels
  * Indication of how easy the question should be
* Question distribution
  * Distribution of K-levels in the exam

## Fundamentals of testing

#### Why do we test?
* Testing and Risk?
  * Minimise Risk.
* Testing and Quality?
  * Want to give an indication of the software quality
* Exhaustive Testing?
  * Testing every option/combination of options.
  * Not really possible, too many options.

#### Key Testing Terms
* **Error** (**Mistake**)
  * Human is responsible
  * Leads to
* **Defect** (**Fault**, **Bug**)
  * Problem with the code
  * Leads to
* **Failure**
  * The project not succeeding


* Effects a defect might have on a project
* Root cause vs. Effect

#### Debugging Vs Testing
* Debugging - Used by developers to identify the cause of bugs or defects in code and undertaking corrections. (What has gone wrong? Can we fix it?)
* Testing - Systematic exploration of a component or system with the main aim of finding and reporting defects. (Has it gone wrong?)

#### Other Things
* Glossary on ISTQB website
* Go by the book

### Seven Testing Principles
1. Testing shows the presence of bugs
2. Exhaustive Testing is impossible
3. Early Testing
  * Start testing as early as Product Requirements
  * Prevent any errors from getting too ingrained
  * Minimise cost to fix
4. Defect Clustering
  * Pareto Principle - 80% of defects are within the same 20% of code
  * Pockets of complexity
5. The pesticide paradox
  * Doing the same test over and over won't catch all the bugs
  * Need to change up testing frequently
6. Testing is context dependant
  * Need your tests to be appropriate to the product you're testing
7. Absence of errors fallacy
  * Just because you can't find errors doesn't mean there aren't any

#### Developer/Tester Mindset
* The approach of a Tester
  * Need to be empathetic towards developers
  * Need to focus on quality/vision
* The approach of a Developer
* Using these different viewpoints to mitigate risk and increase quality


## Testing through the Lifecycle
#### Objectives
* Explain Relationship between development test activities and work products in the SDLC
* Etc.

### Fundamental Test Process
1. Test Planning and Control
2. Test Analysis and Design
  * Can return to 1.
3. Test Implementation and Execution
  * Can return to 2.
4. Evaluating Exit Criteria and Reporting
  * Can return to 2.
5. Test Closure Activities

#### Test Planning and Control
* Determines what is going to be tested
* How is it going to be tested
* Who is doing the testing
* How it will be achieved
* Will also **determine exit criteria**
  * Exit Criteria - What needs to be achieved before the testers can leave
  * Think about Decision/Statement Coverage (Not that common)

#### Test Analysis and Design
* The fine detail of what to test
* Test conditions, cases and procedures
  * Conditions - A characteristic of our software that we can check with a test or set of tests.
  * Cases - The actual tests we're going to be doing - Gets to a start point (Execution Preconditions), Input values to achieve an expected result, leaves the system at an end point (Execution post conditions)
  * Procedures - The methodology for the tests (script)
* **The Test Base is reviewed**
  * Body of knowledge used as the basis for test analysis and design
* We look at how to combine test conditions into test cases

#### Test Implementation and Execution
* Most visible part of testing
* Prioritising test cases
* Creating test suites from collected test cases
  * A set of test cases or test procedures to be executed in a specific test cycle
* Environment set-up
* Log testing activities and defects
  * Write up results in a log (EG: JIRA)
* Running tests

#### Evaluating Exit Criteria and Reporting
* Has the criteria been met to satisfy the stakeholders
* Does the system do as expected
* Determine if more tests need to be made
* Is the system ready for release

#### Test Closure Activities
* Make sure docs are up to date and archived
* Passing over testware to maintenance teams if available
  * Enable Support staff to test the software and resolve issues
* Lessons learnt

### Development Models
Methodology chosen depends on the:
* Nature of the project
* Project schedule
* Resource availability

#### **Waterfall**
*
#### ***V-Model***
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
#### **Agile**


## Test Levels
#### Objectives
* Apply the different test levels (Component, Integration, System, Acceptance) as the appropriate stage in the SDLC with constant reference to characteristics of good testing
* Recognise and compare with examples: functional, non-functional, structural and change related testing
* Etc.

It is important to remember each level of testing has different requirements

### Unit Testing
* AKA: Component/Program/Module Testing
* Each unit of code is usually created in isolation
* Each unit of code will relate to a certain function or area and be *tested by the developer* to make sure it works
* As more code is developed, more and more tests are created

Generally, most system failures will be in a small proportion of modules.

### Integration Testing
* Units are integrated and tested together
* There are two types to remember
  * Big Bang Integration
  * Incremental Integration

#### Incremental Integration
##### Top Down
* High level modules are created first, so a stub code is needed
  * Stub code = filler code to allow testing before some code is created
* Pros
  * Useful for generic software
  * Allow for early demonstrations of product functionality
  * Etc.
##### Bottom Up
* In absence of parent modules, drivers are used
* Pros
  * Higher Accuracy at the granular level
  * Etc.

##### Hybrid

### System Testing
* System testing looks at the behaviour of the system
* Harnesses complete end to end scenarios in the way that the customer would use the system
* A test team must endeavour to apply every agreed input and receive the correct output to exercise the full capabilities of the system

Possible tests (including non-functional):
* GUI
* Usability
* Exception Handling
* Volume
* Scalability
* Ad-Hoc
* Installation
* Recovery
* Performance
* Load
* Security
* Stress

You can't test everything or use every type

What affects the type of system testing you use?
* Size of company
* Time available
* Resources available
* Learning Curve
* Budget

### Acceptance Testing
Testing against User Expectations
* Does the system meet all user requirements?
* This should have been asked frequently throughout the cycle
* Typically verifies the functional fitness of the system for business users
* Note: Acceptance Testing can take place before System Testing starts

A Crucial element for making sure the product will be functional in its perceived environment

Additional aspects to think about at this point are:
* Back-Up
* Disaster Recovery
* Etc.

#### Contract and Regulation Acceptance Testing
* Contractual - Acceptance criteria outlined in a contract
* Regulations - Some industries have rigid regulations that must be adhered to:
  * Government
  * Legal
  * Safety Reasons

Ignorance is not an excuse

#### Alpha/Beta Testing
* Alpha - Performed at the developing site, but not by the developing team.
* Beta - Performed by customers at their own location

Allows for feedback from potential or existing customers


### Types of Testing - High Level
##### Functional, Non-Functional and Structural Testing

* Functional
  * Requirement Specification Based
  * Black-Box - Cannot see the code
  * (Can be done at all levels)
* Non-Functional
  * Performance
  * Usability
  * (Often used to check the readiness of the system)
* Structural
  * Control Flow
  * Menu Structure
  * White-Box - Can see the code
  * (Can be done at all levels)
* Change Related
  * Carried out on a live system

#### Functional (Black Box)
Testing the functions of the system. Verifying a specific action or function of the underlying code works.

#### Non-Functional
Testing of the quality characteristics of the component or system
* Efficiency testing
* Maintainability testing
* Load testing
* Performance testing
* Compatibility Testing
* Scalability Testing
* Stress Testing

#### Structural (White Box)
How the code makes the functionality work. What is happening "under the hood"
* Decision Coverage
* Statement Coverage

### Confirmation, Regression and Maintenance Testing
#### Retesting (Confirmation Testing)
Confirming that changes made successfully fix the issue

#### Regression Testing
Carried out on every other part of the system to check that a fixed defect hasn't changed other parts of the system
* Repeated testing of already tested program
* Performed when software or environment changes
* Based on risk
* Performed at all levels (Functional, Non-Functional, Structural)

#### Change Related Maintenance Testing
Testing in a live environment when there has been:
* Modification
* Migration of Software
* Retirement of Software

Impact analysis (Risk) and Metrics from previous projects are very important in this area
* They help estimate the amount of re-testing and regression testing
* What are the possible consequences?
* What areas will remain unchanged?

Difficulties you may encounter:
* Specifications could be out of date
* People with domain knowledge may no longer be available
* Should not differ much from other test processes


## Static Testing Techniques
#### Objectives
* Explain why and how dynamic testing is different from static testing and their complimentary role in the SDLC
* Identify, with examples, what can be tested using static techniques and explain why
* Recognise and understand reviews and the different levels of formality required (informal, technical, walkthrough, inspection)
* Explain the activities and roles of a formal review process
* Identify the success factors for best practice reviews and highlight key results a review can uncover

### Dynamic Testing Vs Static Testing
* Dynamic - Examination by execution of the code
* Static - Examination without executing the code
  * Involves either reviews of documentation or static code analysis

### What can be inspected?
* Code
* Requirements
* Business Policy
* Strategy
* Test Plans/Designs/Cases

### Reviews and levels of formality
* Informal
  * *Lowest Formality*
  * No Formal Process
  * Not usually documented
  * Inexpensive way to achieve limited benefits
  * May be implemented as Pair Programming
* Walkthrough
  * Led by the author of the document (***Kahoot Question***)
  * Can vary widely in practice from formal to informal
  * Main purpose to enable learning
* Technical Review
  * Documented
  * Usually performed as a peer review led by moderator
  * Can also vary widely from informal to formal
* Inspection
  * *High Formality*
  * Led by trained moderator
  * Pre-Meeting prep is essential
  * Main purpose to find defects
  * Secondary may be process improvement

### Benefits of Static Testing
* Early defect detection and correction
* Fewer defects
* Reduced testing time and cost
* Reduced development timescales
* Etc.

### Formal Review Process
1. Planning
 * Allocate roles
 * Define entry and exit criteria
 * Selecting the parts of documents to be reviewed
 * Checking entry criteria
2. Kick-off
 * Distributing documents
 * Explaining objectives, process and documents to the participants
3. Individual Preparation
 * Individuals review documents
 * Highlight issues
4. Examination/Evaluation/Recording of results
 * Discussing or logging with documented results or minutes
 * Noting defects making recommendation regarding handling the defects making decisions about the defects
 * Examining/Evaluating and recording issues
5. Rework
 * Fixing defects found
 * Recording updated status of defects
6. Follow-up
 * Checking that defects have been addressed
 * Gathering Metrics
 * Checking on Exit Criteria

### Roles in a Formal Review
* Leader/Moderator - Plans Reviews, Chooses participants, conducts meeting, performs follow up.
* Manager - Decides on execution of reviews. Determines whether review process objectives have been met.
* Author - of the document being reviewed. Helps understanding of defects.
* Reviewers/Inspectors - Specialised fault-finding roles
* Scribe - Documents all issues and points made during meeting
* Others - Inspection/review co-ordinator

### What might we find in a review?
* 60% of defects have normally been made before the coding has even started.
* Verification/Validation.
* You find causes rather than faults. This is a positive way to test.
* Security Vulnerabilities
* Programming Standards
* Unreachable (dead) code
* Missing or incorrect logic

### Things to remember
* Each review has clear predefined objectives
* The right people for the review objectives are involved
* Testers are valued reviewers who contribute to the review and also learn about the product which enables them to prepare test earlier
* Defects are welcomed and expressed objectively
* Review is not used for evaluation of the participants
* Review techniques are suitable to the type and level of software work-products and reviewers
* Checklists or roles should be used where appropriate to increase effectiveness or defect identification
* Management support is essential for a good review process
* Emphasis on learning and process improvement

## Test Development and Design
#### Objectives
* Understand why we have test design techniques and what a test basis document is used for
* Differentiate between a test design spec, test case spec and a test procedure spec
* Etc.

To Remember: There are no right or wrong ways

Why do we rely on established test design techniques?
* Help us achieve a given level of acceptance and confidence in the software

What would happen if we didn't use these techniques?
* Amount of testing could spiral out of control

### Test Design
You must consider the context (environment) within which the tests are taking place:
* The Organisation
* The maturity of the development and testing process
* Time/resource constraints
* Safety or regulatory requirements
* The people involved

Why is traceability from test procedures back to specifications important?
* It enables both effective impact analysis when requirements change, and determining requirements coverage for a set of tests

#### Test Design Specification
* Highest level document we create
* Specifies the test conditions for a test item, the detailed test approach and identifies the associated high level test cases
* Template: IEEE829

#### Test Cases

Now that we understand the conditions, we can create the Test Cases

These consist of a set of input values:
* Execution Preconditions
* Expected Results
* Execution Post-Conditions

The Objective of compiling the test case specifications is to specify in detail each test case listed in the test design specification

##### Test Case spec example
* Description
* Preconditions
* Steps
* Input
* Expected Result
* Actual Result
