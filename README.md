# Youtube Test plan

## Revision History

| Date       | Description                        | Author      | Comments                      |
|------------|------------------------------------|-------------|-------------------------------|
| 13.06.2024 | Test Plan pentru versiunea 1.0     | [Nume Autor]| Draft test plan               |
| 15.06.2024 | v1.1                               | [Nume Autor]| Added more details for Test Process |

## Table of Content
1. [Introduction](#introduction)
2. [Project Objective](#project-objective)
3. [Functionalities in Scope](#functionalities-in-scope)
4. [Functionalities and Tests Out of Scope](#functionalities-and-tests-out-of-scope)
5. [Test Process](#test-process)
    - [Test Planning](#test-planning)
    - [Test Analysis](#test-analysis)
    - [Test Design](#test-design)
    - [Test Implementation](#test-implementation)
    - [Test Execution](#test-execution)
    - [Test Closure](#test-closure)
    - [Test Monitoring and Control](#test-monitoring-and-control)
6. [Test Deliverables](#test-deliverables)
7. [Schedule](#schedule)

## Introduction

YouTube is a video-sharing platform. This version will include a limited set of functionalities. Over time, new functionalities will be added to the site.

## Project Objective

Our goal is to increase confidence in the quality of the project as much as possible before releasing it to users.

**Application under test:** YouTube  
**Documentation:** YouTube API Documentation

## Functionalities in Scope

All functionalities of the main YouTube module defined in the business requirements will be tested using the following types of testing: functional testing, GUI testing, API testing. The YouTube web application will be tested on the latest versions of Chrome.

### Functionalities for Manual Testing:
- Sign-up/Sign-in
- Password Recovery
- Account Removal
- Upload Video
- Commenting Feature
- Video Playback
- Search
- Filter Video
- Like/Dislike Video

### Functionalities for Automated Testing:
- Sign-up/Sign-in
- Password Recovery
- Account Deletion
- Search Video
- Video Playback
- Like/Dislike Video
- Search
- Filter Video

## Functionalities and Tests Out of Scope

- Non-functional testing such as stress and performance testing is beyond the scope of this project.
- Only web applications will be tested.
- Security testing (e.g., penetration testing, vulnerability scanning) is not included in this testing cycle.
- Localization and internationalization testing for languages other than English will not be included in this project.

## Test Process

### Test Planning

#### Roles and Responsibilities:
- **[Adrian Pricopie Junior Tester]**: Will test Sign-up/Sign-in, Password Recovery, Account Deletion, Like/Dislike Video.
- **[Robert Furtuna Middle Tester]**: Will test Search, Filter Video, Video Playback.
- **[Ionica Stefan Senior Tester]**: Will test Video Playback, Video Comments, Video Upload.

#### Entry Criteria:
- Smoke tests have been passed.
- The testing environment is functional.
- Roles required for the project are allocated.
- Functional specifications are defined.

#### Exit Criteria:
- 100% of tests have been executed and 95% of them have passed.
- No critical defect is in "Open" status (all remaining defects have low severity).
- Update tests are 100% passed.
- Exploratory testing has been conducted on the main module.

#### Risks:
- **Project Risks**:
  - Limited Resources: Lack of adequate resources (time, personnel, equipment) can delay test execution.
  - Requirement Changes: Business requirements may change during the testing cycle, which could require rework and additional resources.
  - Environmental Issues: Issues related to the configuration or stability of the test environment can delay testing.
  - External Dependencies: Issues with external APIs or other integrations that are not under the control of the testing team can affect testing.
  - New Browser Might Not Be Supported: A new browser might not be compatible, affecting testing.
  - All Remaining Test Cases Are Blocked by an Open Bug: All remaining test cases are blocked by an open bug.
  - Critical Bugs Are Open and They Are Blocking Testing: Critical bugs are open and blocking testing.

- **Product Risks**:
  - Critical Defects: Discovering critical defects late in the testing cycle can negatively impact the release timeline.

### Test Analysis

- Analyze business requirements to ensure all details necessary for creating test conditions are available.
- Write test conditions.
- Plan to run a complete regression test on the current version.

### Test Design

- All test cases are written and reviewed.
- All test cases will be created in Jira as the test management tool.
- Automated tests will be developed using an appropriate testing framework (e.g., Selenium, BDD for GUI testing, pytest for API testing).
- Results of automated tests will be reported and monitored in Jira, facilitating the tracking and management of discovered defects.

### Test Implementation

- All test data is available and reviewed.
- This test run includes only regression testing, where we will run the highest priority tests.
- Test suites are created (Cycle Summary has been created).
- Automated tests will be integrated into the CI/CD pipeline to allow continuous running with every code change, thus ensuring early defect detection.

### Test Execution

- Tests will be executed on the Chrome browser. If time permits, we will extend testing to other browsers.
- Bugs will be created based on failed tests.
- Full regression testing will be performed after changes in the application.
- Retesting will be conducted after a bug is fixed.

### Test Closure

- 100% of tests have been executed and 90% of them have passed.
- No critical defect is in "Open" status.

### Test Monitoring and Control

- Various periodic reports will be generated to reflect the current status of the testing process. In case of major issues, control measures may be taken.
- For automated testing, HTML reports will be generated using pytest.
- For manual testing, Jira will be used for test management and the traceability matrix.

## Test Deliverables

- **Test plan:** Link to the test plan.
- **Test conditions:** We will use the production environment. Testing with new and old accounts is necessary. Test conditions will be exported from Jira and added here.
- **Test cases:** Link to test cases/export from Jira with all written test cases.
- **Daily test summary report:** Link to the daily test summary report (number of tests run today, % of them failed, passed, retested, etc.).
- **Traceability matrix:** Link to the traceability matrix.
- **Test case results:** Link to test case results.
- **Bugs report:** Link to the bugs report.
- **Test completion report:** Link to the test completion report.

## Schedule

- We have 10 days of testing.
- We have 30 test cases.
- To complete the regression run, we should run approximately 3 tests/day.
