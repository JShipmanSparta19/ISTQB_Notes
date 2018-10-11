# Defect Management
### Objectives
* Understand the need for bug detection and apply the defect lifecycle
* Recap terms such as problem, fault, bug, failure and defect
* Determine defect severity and learn how to apply prioritisation to the defects

## Definitions IEEE Standards 1044-2009
* Problem
  * Difficulty or Uncertainty experienced by one or more persons, resulting from an unsatisfactory encounter with a system in use
  * A negative situation to overcome
* Fault
  * A manifestation of an error in software
* Failure
  * Termination of the ability of a product to perform a required function or its inability to perform within previously specified limits
  * An event in which a system or component does not perform a required function within specified limits
* Defect
  * An imperfection or deficiency in a work product where that work product does not meet its requirements or specs and need to be either repaired or replaced

### Bugs
* A bug is a matured term of defect
  * A defect is usually referred to as a bug only if it affects operation of the system and negatively impacts the user of the system
* A defect itself may not have any impact on operation of the system
* All bugs are defects, but not all defects are bugs

#### Reasons for Bug Testing
* Insufficient/Bad Requirements could introduce errors
* Limited time for comprehensive development
* Inexperienced teams
* Coding practices not adhered to
* Human factors
* Little Version Control
* Third-Party Tools
* Changes in requirements
* Level of Software Testing skill

#### Two Main Categories of Bug Testing
* Detection
* Prevention
  * Writing Better Specs
  * Code Review
  * Static Analysis
  * Unit Testing

#### Determining Severity
Categorising:
* Helps determine the efficiency of Test Process
* Helps decide priority of defect
* Bug Tracking process can be made more effective if severity is clearly defined

##### Severity Vs Priority
Severity | Priority
-|-
Blocker | Priority 1
Critical | Priority 2
Major | Priority 3
Normal | Priority 4
Minor | Priority 5
Trivial |
Enhancement |

##### Questions to ask before determining severity

##### Severity Matrix
 | Low Likelihood | High Likelihood
-|-
High Severity | Low impact, but user unfriendly | Data Loss
Low Severity | Cosmetic Error | Impact on minor things, but user can still do work

#### Bug Tracking Problems
* Improper bug logging process
* Use of different bug tracking template
* Improper defect triage process
* Bug tracking tools
* Improper set up of severity and priority
* SPOC (Single Point of Contact)
* No Control of Test Environment

## Tips
* Isolate the defect
* Analyse the defect
  * Supported class of inputs
* Sequence of events
  * List of what doesn't trigger the bug
* Decide early on
* Guide you on amount of work needed
