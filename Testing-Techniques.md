# Testing Techniques
### Objectives
* Explain the characteristics and differences between specification-based testing, structure based testing and experience based testing
* Apply equivalence partitioning, boundary value analysis, decision tables and state transition diagrams/tables
* Explain the concept of use case testing and its benefits
* Describe the importance of code coverage
* Be able to write test case specs
* Assess statement and decision coverage for completeness with respect to defined exit criteria
* Recall reasons for writing test cases based on intuition, experience and knowledge about common defects
* Compare experience based techniques with specification based testing techniques
* Classify test design techniques according to their fitness to a given context for the test basis respective models and software characteristics


## Types of Testing
* Functional - Specification Based, Black-Box
* Non-Functional - Performance, Usability
* Structural - Control Flow, Menu Structure, White-Box
* Change Related - Carried out on a live system

## Functional Testing
* Examines the functionality of an application without knowledge of its internal structures
* It is based entirely on the software requirements and specifications

### Techniques we will be looking at
* Sanity/Smoke Check
* Decision Table Testing
* State Transition Testing
* Equivalence Partitioning
* Boundary Value Analysis
* Use Case Testing

### Sanity Check/Smoke Test
* Smoke Test - Aim is not to find defects, but check for system health
* Sanity Check - Makes sure the bugs reported in previous builds are fixed for this release before doing a full regression test

Acceptable in the Integration/System/Acceptance Testing levels

### Decision Table Testing
Compact and precise way of modelling complex logic

Lists all conditions that can occur + consequences

Conditions | Sets of Conditions
-|-
Actions | Action Entries

* Sets of conditions are Bool values that make up the different possible combinations of conditions
* Action Entries are check marks, representing which of the actions in a given column are to be performed

#### Infeasibility
Certain combinations are logically impossible.

Sometimes we want to test an infeasible test condition to make sure it can't happen

### State Transition Testing
* When a system is represented as being in one state and transitions from that state to another
* The transformations are determined by the rules of the system
* This means we can follow these rules to create a diagram that represents the change of transitions and thus a test to see if it works

Goal: Finding situations where the wrong action or the wrong new state occurs in response to a particular event.

As testers, we report these problems all the time as bugs.

When a system should only be in a finite number of states, we can use transition testing techniques to create our tests

EG: A door transitions between the open and closed state

* States - How something exists at that time
* Transitions - The change from one state to another.
  * Triggered by...
* Inputs/Events - What triggers a state transition
* Actions - Actions that can result from a transition

#### 0-1-2-3 Switch Summary
* If every valid transition is tested, this is known as "0-switch" coverage
* You could also test a series of transitions through more than one state
* If you covered all of the pairs of two valid transitions, you would have "1-switch" coverage
* Covering the sets of 3 transitions would give "2-switch" coverage, etc.

#### Process for state transition testing
* Draw state transition diagram
* Determine start state, input, output and finish state
* Determine coverage level to be achieved
* Draw testing tree
* Define tests

### Equivalence Partitioning (Equivalence Classes)

* Rather than trying to test infinite amounts of inputs, strategically sample them
* Divides a set of test conditions into partitions that can be considered the same
* At least one value is tested from all classes
* Does not consider "silly" inputs (EG: minus values when inputs should only be positive)

### Boundary Value Analysis

* Similar to Equivalence Partitioning, but focuses on numbers close to the boundaries of the partitions
* Designed to catch common errors at these boundaries, particularly if related to the transition between the boundaries
* Does consider "silly" inputs

### Use Case Testing

Describes interactions between 'actors' and the system

* Characters/Actors
  * Users can play many roles with respect to a system
  * If we do not understand all the roles a user plays, then we cannot understand the system
  * It can be diagrammatical or as a scenario

Advantages:
* Very useful when testing process flows and business rules
* Very effective in defining acceptance tests as the use case usually represents how the system will be used
* It is often good practice to write a test case representing each use case

Can also define Use Cases as Steps

Tabulating Use Cases:
* Be to the point
* Assume the system has not been built

Disadvantages:
* Tying services to users may make the system too rigid
* If you do not have a wide selection of personnel in the Use Case team, a narrow focus can obscure all the services a user requires
* Focus can be swayed to how the user will use the system rather than the services the user needs
* Time pressure and need for results can create a situation where we only analyse the users

Success Factors:
* Size of team
  * Want a small team made up of the right characters - Focused, but balanced
  * Involve as many stakeholders as possible
* Make sure they have a shared vision, everyone needs to be on the same page
* Know when to stop
  * Stop developing Use Cases once they are complete and satisfactorily meet audience needs
  * Have a good Definition of Done
  * Establish a boundary between the system and its environment
* Review Use Cases
  * At multiple points through the exercise]

## Experience Based

* Error Guessing
  * A test design technique where the experience of the tester is used to anticipate what defects might be present in the component or system under test as a result of errors made and to design tests specifically to expose them
* Defect and Failure Lists
  * Help identify areas susceptible to problems
* Fault Attack
  * This approach is to list possible errors and design tests around that list
* Exploratory Testing
  * An informal test design technique where the tester actively controls the design of the tests as those tests are performed and uses information gained while testing to design new and better tests

### Exploratory Testing

* One of the most powerful forms of testing
  * Has the bare minimum of a plan
* Important tool in the hands of SMEs (Subject Matter Experts)
* It is especially suited to web app development in agile methods

Advantages:
* It doesn't require much preparation
* Testers report a large proportion of bugs via this method

Disadvantages:
* There is no review of test planning, an experience user of the system may not be an experienced tester
* Testers have to remember the exact steps they took to create a defect - otherwise reproduction may be difficult

#### Five Key Elements
* Product Exploration
* Test Design
* Test Execution
* Heuristics - AI/Learning
* Reviewable Results


* Still need a well defined structure rather than having a scatter gun approach
* Also need to be able to define how complete your exploratory testing was
* This can be attained through Heuristics/Mnemonics

#### SFDPOT - San Francisco Depot (James Bach)
* Structure - What the Product is
  * Number of programs?
  * Can it be tested module by module?
  * Documentation?
  * What was it built with?
* Function - What the Product does
  * What is the UI like?
  * What is it meant to do?
  * Does it interface with other systems?
* Data - What it Processes
  * What kind of data does it input/output? (Are there already examples of this?)
  * Are there specific rules surrounding the input/output?
* Platform - What it Depends on
  * Does the environment have to be configured in a special way?
  * What is the OS it runs on?
* Operations - How it Will be Used
  * Who is it used by?
  * Where do they use it?
  * What do they use it for?
  * Are there different methods that different users will utilise?
* Time
  * How Long Does it Take to do What You Need to do?
  * Affected by Timezones or DST?

## White-Box Testing

* AKA: Clear, Glass, Open, Transparent, Structural
* Tests internal structures as opposed to Functional Testing
* Usually done at Unit level, but can be applied to Integration and System
* Focus primarily on
  * Strengthening Security
  * Flow of Input/Output through the Application
  * Improving Design and Usability
* Crucial to already have some knowledge of the code language used to create the software

### Types
* Decision (or Branch) Coverage
* Statement Coverage

#### Branch/Decision Coverage
* Check how many possible branches from decisions in the code have been executed at least once
* Decision Coverage Testing: White Box test design technique in which test cases are designed to execute condition outcomes and decision outcomes
* A Decision is any point where the flow branches (Anything with multiple outputs)
* Decision tests need to go down each flow branch at least once
* 100% Decision Coverage => 100% Statement Coverage

#### Statement Coverage
* Check how many statements in the code have been executed at least once
* Statement Testing: White Box test design technique in which test cases are designed to execute statements
* A Statement is anything that we are getting the processor to do (Anything with a single output)
* Statement Tests need to pass through each Statement at least once

#### Path Coverage
* Check every possible path
* Need to test every possible combination of decisions
* 100% Path Coverage => 100% Decision Coverage

### Code and Psuedo-Code
Part of Code Coverage used to determine which parts of code have been executed

#### Psuedo-Code
A way of writing code while stripping out most of the syntax and other forms of language dependence

#### Sequential Code
* Code where there are no decision points - code is executed line by line
* Only ever need one test case for this

## Choosing Test Techniques
* Type of System
  * Is it safety critical?
  * Is it a financial system?
  * Is it web/cloud based?
* Regulatory Standards
* Customer/Contractual Requirements
* Level of Risk
  * Functional
  * Non-Functional
  * Structural
  * SLA (Service Level Agreement)
* Test Objective
  * What are we trying to demonstrate?
* Available Documentation
* Knowledge of the Testers
* Time/Budget
* Type of Dev Lifecycle
* Use of Case Models
* Previous Experience of Defects

Structural/White-Box | Specification/Black Box  | Experience Based
---------------------|--------------------------|-----------------
Decision Coverage    | Sanity/Smoke Check       | Error Guessing
Statement Coverage   | Decision Table Testing   | Defect & Failure Lists
Path Coverage        | State Transition Testing | Fault Attack
                     | Equivalence Partitioning | Exploratory Testing
                     | Boundary Value Analysis  |
                     | Use Case Testing         |
