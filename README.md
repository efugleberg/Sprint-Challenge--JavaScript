# Sprint Challenge: JavaScript Fundamentals
Eric
This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a survey of problems. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied variables, functions, object literals, arrays, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a survey of JavaScript problems.

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your PM and Instructor in your cohort help channel on Slack. Your work reflects your proficiency in JavaScript fundamentals.

You have three hours to complete this challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your project manager.

## Description

You will notice there are several JavaScript files being brought into the index.html file.  Each of those files contain JavaScript problems you need to solve.  If you get stuck on something, skip over it and come back to it later.

In meeting the minimum viable product (MVP) specifications listed below, you should have a console full of correct responses to the problems given.

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

1. Describe the biggest difference between `.forEach` & `.map`.

.forEach: This iterates over a list and applies some operation with side effects to each list member (example: saving every list item to the database). .forEach doesn’t actually return anything. It just calls the function for each array element and then it’s done. So whatever you return within that called function is simply discarded

.map: This iterates over a list, transforms each member of that list, and returns another list of the same size with the transformed members (example: transforming list of strings to uppercase).  On the other hand, .map will similarly call the function for each array element but instead of discarding its return value, it will capture it and build a new array of those return values.

So, biggest difference is that .forEach doesn’t return anything unless you specifically push data to a new array and .map automatically returns a new array with the function .map performs on the array.

2. What is the difference between a function and a method?

A function is a piece of code that is called by name.  It can be passed data to operate on and can optionally return data. A method is a piece of code that is called by a name that is associated with an object. In most respects it is identical to a function except for two key differences:

A method is implicitly passed the object on which it was called.
A method is able to operate on data that is contained within the class (remembering that an object is an instance of a class - the class is the definition, the object is an instance of that data).

3. What is closure?

Closure is a JavaScript feature which allows us to write cleaner, more concise code.  A closure is an inner function that has access to the outer (enclosing) function’s variables.  You create a closure by adding a function inside another function.

4. Describe the four rules of the 'this' keyword.

1) Window/Global Object Binding:  The value of "this" will be the window/console Object.  In function call, 'this' points out at global object.
2) Implicit Binding:  Whenever a function is called by a preceding dot, the object before that dot is 'this'.  Before going to global object properties,
'this' goes into its object context to which it has binding because the object has a property which is storing a function as a method - thus, it's implicitly bound. 'This' does not search for a global object because object context has higher precedence than global object and is found when the function is called --> this bypasses the need to search in the global object.
3) New Binding: Occurs when a constructor function is used.  'This' refers to the specific instance of the object that is created and returned by a           constructor function.
4)  Explicit Binding:  Whenever JavaScript's call or apply method is used, 'this' is explicitly defined. Explicit binding occurs when we call functions via object AND explicitly bind a specific object in the function call.


5. Why do we need super() in an extended class?

Super() goes into the ‘Parent’ class and pushes all of the key: value pair templates and methods to the class using the extension.  Prior to applying super(), our ‘child’ class does not have the key: value pairs from the ‘parent’ class.  After, super() is applied, our ‘child’ class inherits the key: value pair templates from the ‘parent’ class.

## Project Set up

Follow these steps to set up and work on your project:

- [x] Create a forked copy of this project.
- [x] Add PM as collaborator on Github.
- [x] Clone your OWN version of Repo (Not Lambda's by mistake!).
- [x] Create a new Branch on the clone: git checkout -b `<firstName-lastName>`.
- [x] Create a pull request before you start working on the project requirements.  You will continuously push your updates throughout the project.
- [x] You are now ready to build this project with your preferred IDE
- [x] Implement the project on your Branch, committing changes regularly.
- [x] Push commits: git push origin `<firstName-lastName>`.

Follow these steps for completing your project:

- [x] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo).
- [x] Add your Project Manager as a Reviewer on the Pull-request
- [x] PM then will count the HW as done by  merging the branch back into master.


## Minimum Viable Product

Your finished project must include all of the following requirements:

**Pro tip for this challenge: If something seems like it isn't working locally, copy and paste your code up to codepen and take another look at the console.**

## Task 1: Objects and Arrays
Test your knowledge of objects and arrays. 
* [x] Use the [objects-arrays.js](challenges/objects-arrays.js) link to get started.  Read the instructions carefully!

## Task 2: Functions
This challenge takes a look at callbacks and closures as well as scope. 
* [x] Use the [functions.js](challenges/functions.js) link to get started. Read the instructions carefully!

## Task 3: Prototypes
Create constructors, bind methods, and create cuboids in this prototypes challenge.
* [x] Use the [prototypes.js](challenges/prototypes.js) link to get started. Read the instructions carefully!

## Task 4: Classes
Once you have completed the prototypes challenge, it's time to convert all your hard work into classes.
* [x] Use the [classes.js](challenges/classes.js) link to get started. Read the instructions carefully!

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Stretch Problems

There are a few stretch problems found throughout the files, don't work on them until you are finished with MVP requirements!
