# CS151 PROGRAMMING ASSIGNMENT #3  
60  POINTS   (10pts design, 50pts final)  
DESIGN DUE: 10/11/17  
FINAL DUE: 10/18/17  

## PROBLEM 
Create a program that will calculate various sports statistics for the user, based on the user’s choice of statistic. 

## PURPOSE OF THE ASSIGNMENT
The purpose of this assignment is to give you practice with

1. input & output
2. decision making
3. function design and implementation
4. error checking

## REQUIREMENTS ANALYSIS
The first stage in your programming assignment is the requirements analysis stage.  You need to make sure you understand the below requirements for what your program needs to do. Your program will give the user the option of calculating statistics relevant to three sports. You must do the calculations for the following sports in your program: 

* Quarterback rating in American football  
  * The quarterback rating determines how good a quarterback is in passing (throwing) a football. A perfect passer rating in the NFL is considered to be a 158.3.  
  * QB rating = 100 * [5(completions/attempts – 0.3) + 0.25(passing_yards/attempts-3) + 20(touchdown_passes/attempts) + 2.375 – (25 * interceptions/attempts)]/6  
  * Note that attempts means the number of passing attempts made, and is the same number used throughout the equation.  
  * You will want to tell the user whether or not the quarterback is a perfect passer.  
  
* Calculate the score for a team in a game of Quidditch as described by the International Quidditch Association (http://www.iqasport.com/). 
  * A goal is scored by propelling the quaffle through a hoop. The team earns 10 points per goal.
  * If the team has caught the snitch, the team earns an additional 30 points 
  
* Calculate the final score for a gymnast on any apparatus. 
  * Assume there are 6 scores (we’re simplifying slightly from the real world). One score is on difficulty. The other 5 scores are on execution. All scores are between 0 and 10. Of the execution scores, the highest and lowest are dropped. The final score is acquired by adding the difficulty score to the average of the execution scores.

In your program, you must do some basic error checking: check if you are going to divide by zero when relevant, and don’t do the calculation if that’s the case; and before typecasting input to an int, check that it is only digits, and don’t typecast or do the calculation otherwise. In any case where an error is detected, output that it was an error, and don’t continue the calculation – you may output a zero for the result of the calculation.

## DESIGN
The second stage is to design your solution based on the requirements:

1. Determine the tasks being accomplished in your program. Each of these should be a function.
2. Remember that the user is only going to do ONE of the sports statistics calculations, although your program can do all three of them. They choose which one to do.
3. Write an algorithm for each function. This algorithm includes parameters, calculations, and returned values. In general your function will NOT output anything, except perhaps error messages when invalid input is given; your main program should do all of the output of results. Results from functions should be returned.
4. Make the main part of your program be in a “main” function. The main function never takes parameters, and does not return anything. The main function will call most of your other functions.
5. Double check that you included all of the requirements.

*NOTE:* There are no aspects of this program that you can google how to solve. The only appropriate googling will be if you want to understand a sport or its calculations better. You MUST write your own code to find the min/max for gymnastics.

You may find it helpful the first time to start on your algorithm first, and then break it up into functions later. But you need to have it written in terms of functions for the design submission. 

**DESIGN SUBMISSION: 10/11/17**

Submit to GitHub: the algorithm for your program in designInitial.txt. The general format for each function is given. You can copy/paste the starting point (name, parameters, return, algorithm headers) for as many functions as you need to define for your problem.

***Remember to double check on github.com that your files pushed. If they didn’t, you need to push them. I can only see what is on github.com, not what is only on your computer.***


## PROGRAMMING REQUIREMENTS
After your design is complete and correct, it’s time to start programming and then testing:

* Fix design issues: If there were issues with your design, either not meeting requirements or in the format, fix that before you start writing your code.
* Implementation: Write your program following the requirements and based on your design.
  * Follow good usability/HCI principles in your input and output (make it clear the type of input you are asking for)
  * Follow good use of functions
  * Remember to define functions before they are used (so if function A calls function B, you need to define function B first in your program)
  * Remember to state the purpose of the program
* Testing: Make sure it works correctly; give it sample input, and check that the output is correct.
  * Create a partial flowchart for your program. You only need to show the details for 1 sport’s calculations. For the other 2 sports, just draw a box and state “calculations for X” where X is replaced with the name of the sport. 
  * Label the control paths in your flowchart. For each control path related to the sport in your flowchart, list a test case.
  * Test your program using the test cases. You ALSO need to make sure you test your other sport calculations even though they aren’t part of your flowchart. If it doesn’t give the expected output, find the error and fix it. You are expected to turn in a fully functioning program without errors.

## ASSIGNMENT REMINDERS
Follow the programming assignment requirements document for comments, formatting, etc.

Recall that you may not do someone else’s work, or have someone else do your work. Sharing of solutions is an honor code violation. This includes someone who is not in the class, including a tutor, writing any or all of your algorithm or code or dictating to you how to do it. As everyone in the class is solving the same problem, no code may change hands. See the syllabus for details or ask the professor if you are unsure.

## EXTRA CREDIT (only if everything else works)
If you choose to do extra credit, it must be submitted in a separate file with “extraCredit” in the file name. 

Each of the following extra credit options will earn you extra credit. You can do either or both of them:
1.	Add error checking to the gymnastics calculation so that the calculation is only done if the score is between 0 and 10.
2.	Design a function that allows the user to keep trying to input an int when an int was asked for, until they do so. Use this function wherever you checked for an int in the original program.


## FINAL SUBMISSION   
* On paper in class:
  * Your .py file
  * Your flow chart
* To Moodle:
  * Your .py file
  * Your extra credit .py file if you did the extra credit (make sure “extraCredit” is in the filename)
  * Your final algorithm, including the changes you made based on the design feedback in designFinal.txt
  * Your test cases based on your flowchart in testcases.txt. You should have at least 1 test case per control path, using boundary values (see notes #7).
* To github:
  * Your .py file

***Remember to double check on github.com that your files pushed. If they didn’t, you need to push them. I can only see what is on github.com, not what is only on your computer.***

