Math Atlas
===========

Version guide
--------------------------------

Current version: 0.0.13
^^^^^^^^^^^^^^^^^^^^^^^
We are almost done with generating all the question content (left with implementation of qn1301). In between updates we have completed MF26 and the grid
selection layout for questions (along with relevant SVGs). The implementation of the two classes: studentInput (fraction and integer modes) and studentRadio (for MCQ)
has greatly enhanced productivity.

Work left to do:

*   Home page
*   Implement random generated question
*   About page
*   Final feature: save progress into local storage and display statistics
*   Bugs and revision: qn0101 check marks, qn0501 bug fix
*   Final round of testing
*   Implementation of cordova (back button?)
*   Feedback page
*   Documentation
*   Android build
*   Web version

Previous versions: 
^^^^^^^^^^^^^^^^^^^^

Version: 0.0.7
~~~~~~~~~~~~~~~
We have built and tested questions 0101 to 0601. Question 0701 is built and pending testing. Starting to design question 0801 (refer to Math Bounty Question section). 

Version: 0.0.6
~~~~~~~~~~~~~~~
We have built and tested questions 0101 to 0501. Question 0601 is built and pending testing. Starting to design question 0701 (refer to Math Bounty Question section). 

Version: 0.0.5
~~~~~~~~~~~~~~~
We have built and tested questions 0101 to 0401. Question 0501 is built and pending testing. Starting to design question 0601 (refer to Math Bounty Question section). New code we're looking forward to implementing: (1) SVG diagrams! (2) writing an object to handle student inputs to speed things up. 

Version 0.0.4
~~~~~~~~~~~~~~
We have built and tested questions 0101 to 0401. Up until 0501 part 1, we were using plain javascript. From 0501 part 2 onwards, we will transition to using typescript. To guarantee backwards compatibility, some functions are repeated in the new typescript files. For such functions, we will append a "Y" behind the file name. Also from 0501 part 2 we implement the fraction object class to handle fractions in our code.