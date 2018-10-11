# Static Testing Techniques
### Objectives
* Explain why and how dynamic testing is different from static testing and their complimentary role in the SDLC
* Identify, with examples, what can be tested using static techniques and explain why
* Recognise and understand reviews and the different levels of formality required (informal, technical, walkthrough, inspection)
* Explain the activities and roles of a formal review process
* Identify the success factors for best practice reviews and highlight key results a review can uncover

## Dynamic Testing Vs Static Testing
* Dynamic - Examination by execution of the code
* Static - Examination without executing the code
  * Involves either reviews of documentation or static code analysis

## What can be inspected?
* Code
* Requirements
* Business Policy
* Strategy
* Test Plans/Designs/Cases

## Reviews and levels of formality
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

## Benefits of Static Testing
* Early defect detection and correction
* Fewer defects
* Reduced testing time and cost
* Reduced development timescales
* Etc.

## Formal Review Process
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

## Roles in a Formal Review
* Leader/Moderator - Plans Reviews, Chooses participants, conducts meeting, performs follow up.
* Manager - Decides on execution of reviews. Determines whether review process objectives have been met.
* Author - of the document being reviewed. Helps understanding of defects.
* Reviewers/Inspectors - Specialised fault-finding roles
* Scribe - Documents all issues and points made during meeting
* Others - Inspection/review co-ordinator

## What might we find in a review?
* 60% of defects have normally been made before the coding has even started.
* Verification/Validation.
* You find causes rather than faults. This is a positive way to test.
* Security Vulnerabilities
* Programming Standards
* Unreachable (dead) code
* Missing or incorrect logic

## Things to remember
* Each review has clear predefined objectives
* The right people for the review objectives are involved
* Testers are valued reviewers who contribute to the review and also learn about the product which enables them to prepare test earlier
* Defects are welcomed and expressed objectively
* Review is not used for evaluation of the participants
* Review techniques are suitable to the type and level of software work-products and reviewers
* Checklists or roles should be used where appropriate to increase effectiveness or defect identification
* Management support is essential for a good review process
* Emphasis on learning and process improvement
