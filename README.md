# Argument-Parser

## Introduction

This project was a group term project for my Software Engineering I course. The goal was to create a command line argument parser using test-driven development and the agile methodology, Scrum. Over the course of five 2-week sprints, we attended four meetings a week, each consisting of a 15 minute Scrum and an hour of working on the code in groups and individually.  

### Tools Used

* **Git** - used for source control
  * *Github* - used as a host for our source control repository
* **Gradle** - used for build automation
* **Robot Framework** - used for acceptance test automation
* **Trello** - used to organize our product backlog and create the sprint backlog


## Classes

* **Command Line Argument** - abstraction of a general argument that can be parsed from the command line. Both positional and named arguments have a name, description, data type, and value. All arguments also have the options of holding multiple values, and can be restricted to specific values.
* **Argument** - extension of the Command Line Argument, specifically dealing with positional arguments. These arguments are required.
* **Optional Argument** - extension of the Command Line Argument, specifically dealing with named arguments.
* **Argument Parser** - houses the argument parser class, which parses arguments from the command line.
* **XML Parser** - an implementation of Argument Parser which deals specifically with XML files. 
* There were also a few exception classes.

## Samples 

### Unit Tests

We created unit tests for 4 of our 5 classes (not including exception classes). In the final sprint we ended up having was 67 unit tests. By the end of the project, we had 94% code coverage, or 94% of the code being tested by unit tests. 

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Overall%20Code%20Coverage.png "Overall Code Coverage")

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Class%20Code%20Coverage.png "Class by Class Code Coverage")

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Argument%20Code%20Coverage.png "Argument Method by Method Code Coverage")

At the end of the project, all of the tests were passing. Below is an overview of all the test classes. I included an overview of the tests from the ArgumentTest class, which tests the basic functions of a positional argument.

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/UnitTestResults.png "Overall Unit Test Results")

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/ArgumentClassUnitTestResults.png "Argument Class Test Results")

The following code snippet shows a unit test designed to add 3 arguments to the list of arguments, then try to parse a simulation of a command line input. If the parse is successful, then the values passed in will be assigned to the specified arguments declared in the beginning of the test.

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Parse%20Argument%20Test.png "Parse Argument Test")

### Acceptance Tests

We created 8 acceptance tests to ensure that our program performed to the project specifications.

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Acceptance%20Test%20Overview.png "Acceptance Test Overview")

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Acceptance%20Test%20Details.png "Acceptance Test Details")

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Acceptance%20Test%201%20Details.png "Acceptance Test 1 Details")

Below is an example of an acceptance test from the Feature1Keywords.txt file. 

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Test1Keywords.png "Acceptance Test 1 Keywords")

### Documentation

We created documentation for our project using Javadoc. All classes, including exceptions, are covered in the documentation, as well as the enumeration we created for the argument data type.

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Documentation.png "Documentation Overview")

### Sample Main

Below is a sample main class designed to be a volume calculator. There are 3 positional arguments, length, width, and height. When the program is run, it reads the arguments that were entered into the command line, and tries to parse the arguments based on the specified data type. If the parsing is successful, it then calculates the volume. 

![alt text] (https://github.com/nikkipruitt182/Argument-Parser/blob/master/Read%20Me%20Images/Sample%20Main.png "Sample Main")

## Acknowledgements
Alix Rosarion, Sari Sabouh, and Kris Daye are co-contributors to this project. 