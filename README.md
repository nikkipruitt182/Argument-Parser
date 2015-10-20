# Argument-Parser

## Introduction

This project was a group term project for my Software Engineering I course. The goal was to create a command line argument parser using test-driven development and the agile methodolgy, Scrum. Over the course of 5 2-week sprints, we attended 4 meetings a week, each consisting of a 15 minute Scrum and an hour of working on the code in groups and individually.  

### Tools Used

* **Git** - used for source control.
  * *Github* - used as a host for our source control repository.
* **Gradle** - used for build automation. 
* **Robot Framework** - used for acceptance test automation.
* **Trello** - used to organize our product backlog and create the sprint backlog.


## Classes

* **Command Line Argument** - abstraction of a general argument that can be parsed from the command line. Both positional and named arguments have a name, description, data type, and value. All arguments also have the options of holding multiple values, and can be restricted to specific values.
* **Argument** - extension of the Command Line Argument, specifically dealing with positional arguments. These arguments are required.
* **Optional Argument** - extension of the Command Line Argument, specifically dealing with named arguments.
* **Argument Parser** - houses the argument parser class, which parses arguments from the command line.
* **XML Parser** - an implementation of Argument Parser which deals specifcially with XML files. 
* There were also a few exception classes.

## Samples 

### Unit Tests

We created unit tests for 4 of our 5 classes (not including exception classes). The final unit tests count was 67 tests. By the end of the project, we had 94% of the code coverage, or 94% of the code being tested by unit tests. 

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Overall%20Code%20Coverage.png "Overall Code Coverage")

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Class%20Code%20Coverage.png "Class by Class Code Coverage")

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Argument%20Code%20Coverage.png "Argument Method by Method Code Coverage")

At the end of the project, all of the tests we had written were passing. Below is an overview of all the test classes, as well as an overview of the tests from the ArgumentTest class, which tested the basic functions of an argument.

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/UnitTestResults.png "Overall Unit Test Results")

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/ArgumentClassUnitTestResults.png "Argument Class Test Results")

The following code snippet shows a unit test that is designed to add 3 arguments to the list of arguments, then try to parse a simulation of a command line input. If the parse is successful, then the values passed in will be assigned to the arguments specified at the beginning of the test.


### Acceptance Tests

We created 8 acceptance tests to ensure that our program performed the correct function.

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Acceptance%20Test%20Overview.png "Acceptance Test Overview")

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Acceptance%20Test%20Details.png "Acceptance Test Details")

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Acceptance%20Test%201%20Details.png "Acceptance Test 1 Details")

### Documentation

We also created documentation for our project using Javadoc. All classes, including expections, are covered in the documentation, as well as the enumeration we created for the argument data type.

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Documentation.png "Documentation Overview")

## Acknowledgements
Alix Rosarion, Sari Sbouh, Kris Daye, Steven Dudchock, and Yi Chen are co-contributors to this project. 