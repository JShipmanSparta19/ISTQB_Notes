# Test Levels
### Objectives
* Apply the different test levels (Component, Integration, System, Acceptance) as the appropriate stage in the SDLC with constant reference to characteristics of good testing
* Recognise and compare with examples: functional, non-functional, structural and change related testing
* Etc.

It is important to remember each level of testing has different requirements

## Unit Testing
* AKA: Component/Program/Module Testing
* Each unit of code is usually created in isolation
* Each unit of code will relate to a certain function or area and be *tested by the developer* to make sure it works
* As more code is developed, more and more tests are created

Generally, most system failures will be in a small proportion of modules.

## Integration Testing
* Units are integrated and tested together
* There are two types to remember
  * Big Bang Integration
  * Incremental Integration

### Incremental Integration
#### Top Down
* High level modules are created first, so a stub code is needed
  * Stub code = filler code to allow testing before some code is created
* Pros
  * Useful for generic software
  * Allow for early demonstrations of product functionality
  * Etc.
#### Bottom Up
* In absence of parent modules, drivers are used
* Pros
  * Higher Accuracy at the granular level
  * Etc.

#### Hybrid

## System Testing
* System testing looks at the behaviour of the system
* Harnesses complete *end to end* scenarios in the way that the customer would use the system
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

## Acceptance Testing
Testing against User Expectations
* Does the system meet all user requirements?
* This should have been asked frequently throughout the cycle
* Typically verifies the functional fitness of the system for business users
* Note: Acceptance Testing can take place before System Testing starts

A Crucial element for making sure the product will be functional in its perceived environment

Additional aspects to think about at this point are:
* Back-Up
* Disaster Recovery
* End User Training
* Maintenance Procedures
* Security Procedures

### Contract and Regulation Acceptance Testing
* Contractual - Acceptance criteria outlined in a contract
* Regulations - Some industries have rigid regulations that must be adhered to:
  * Government
  * Legal
  * Safety Reasons

Ignorance is not an excuse

### Alpha/Beta Testing
* Alpha - Performed at the developing site, but not by the developing team.
* Beta - Performed by customers at their own location

Allows for feedback from potential or existing customers


## Types of Testing - High Level
#### Functional, Non-Functional and Structural Testing

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

### Functional (Black Box)
Testing the functions of the system. Verifying a specific action or function of the underlying code works. (All levels)

### Non-Functional
Testing of the quality characteristics of the component or system
* Efficiency testing
* Maintainability testing
* Load testing
* Performance testing
* Compatibility Testing
* Scalability Testing
* Stress Testing

### Structural (White Box)
How the code makes the functionality work. What is happening "under the hood". (All levels)
* Decision Coverage
* Statement Coverage

## Confirmation, Regression and Maintenance Testing
### Retesting (Confirmation Testing)
Confirming that changes made successfully fix the issue

### Regression Testing
Carried out on every other part of the system to check that a fixed defect hasn't changed other parts of the system
* Repeated testing of already tested program
* Performed when software or environment changes
* Based on risk
* Performed at all levels (Functional, Non-Functional, Structural)

### Change Related Maintenance Testing
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
