#Problem Solving Curriculum: Introduction

1. Use Polya's Problem solving tecniques:
  - understand the Problem
  - devise a plan
  - carry out the plan
  - look back

#Applying Polya's Techniques to Software

1. Identify Inputs and outputs (link)
  - First, verify what they are
  - ask about what type of input they are (string, boolean, array, etc). This will help identify what boilerplate code to use
  - also identify which inputs are required and which are optional, and for optional ones what their default value might be.
  - this relates to #1 in Polyas method.

Determine inputs and outputs, and ask what if questions in apps:
- look at wireframes to see what data users enter and how it will be used. Look at api's and existing data sources. Determine how it's coming in (web sockets, ETL, HTTP), and how it's being served (api, user-facing pages?)
- If there's a user interface, What if a user leaves a field blank? What if a user double clicks a button?
- What if an API goes down? What if a client starts dosing a system?
- For Whiteboard interviews:
  - what parameters does the function take?
  - write down sample inputs and outputs
  - look for basic questions about ranges/overflows. What if the start date is later than the end date?

#Whiteboard Interview Prep (groups)

Objectives:
1. Ask one or more what-if questions about edge cases
2. Propose two or more solutions
3. Stake your claim - choose one solution to recommend, and why

#Rationale:

In the real world, data inputs are usually extremely complex. A good whiteboard interviewer is looking for your problem solving skills.

#How it works

- This relates to step 1 in Polya's method(understand the problem).
- It's up to you to ask what if questions
- what if an email has whitespace at the beginning or end?
- what if there are upper or lowercase letters?
- should we lock people out after many failed attempts?
- Things to look out for:
  - things being out of bounds in an array?
  - missing parameters
  - things out of order
  - things have mis-matched lengths
  - divide by zero errors
- assume there is a hidden requirement until you've confirmed you're good

#Propose a few solutions

- Every time you ask what happens when...
  - follow up with options/guesses and explain why
- ask if there's anything you've missed before writing code

#Stake a claim

- show multiple possibilities
- stake a claim with reason
- doing nothing may be an option
  - (what does this mean)

#Do's and dont's

- always propose solutions/options when talking about what you could do
- avoid menial type checking: what if you don't pass anything into the function? what if you pass a number instead of an array?
- avoid asking interviewer what to do

#Whiteboard Interviews - Verbalizing Solutions

- Objectives: verbalize your solution before starting to write
- mention two ways to solve a problem if and only if: you can think of more than one solution,
- you can deliver on both

# Remember > understand > apply > analyze > evaluate > create

#How it works:

- this relates to step 2 in polya's method (devise a plan)

Before you put a marker on the board...

- Describe what you'll do in a couple sentences

- sometimes there are options available to you
  - store data in arrays or objects
  - use built in methods or not
  - foreach, filter, map, or for loops
  - use recursion or loops
  - write brute-force solutions that are inefficient or write more optimized solutions
  - write a big function, or split it into multiple functions

#"Sandwich" Code

#Objectives

- Identify sensible defaults for each primitive type
- which parts are boilerplate and which require thought
- write boilerplate code from memory

#Rationale

- code can be either boilerplate code or interesting code
- boilerplate code includes things like function/method/class definitions, brackets, etc.
- everything that goes inside this is interesting
- this helps decreasing syntax errors and corrects indentation
- this also frees up your thinking for the tough stuff

#this is step 3 in polyas method

- with all this, you'll have enough info to write class/method/function definitions with inputs, initialize a return value, and return a return value

#A good formula:

- add a sandwich of the function
  - identify inputs/outputs
  - use problem description to come up with a name for the function
  - use inputs to Determine which parameters to add
  - close braces and parens correctly.
- add a sandwhich for the result variable
  - declare, initialize result
  - use type of output to determine default value
  - return the result
- add a sandwich for working with the input
  - iterate over the input
  - note that you'll do something with each value in the iteration, as well as the result (ex. accumulating it)

- give your return variable a default value to help you remember ('', 0, [], {}, true/false)

#Caveats

- remember this won't always work (not always needing iteration)
- sometimes you don't actually need a result variable

#testing whiteboard code

- employ a methodical process at a whiteboard interviewer
- run through code with actual values, check every iteration

#Rationale
- ideally, these should check your problem solving skills (you can think like an interpreter)
- you are methodical

#this relates to step four in poly's method

#PROTIP: "Test the code you wrote, not the code you thought you wrote" <-- Experienced Google Interviewer

- check correctness and dryness

#getting the most out of warmups

Objectives: use polya's methods to solve warmups
- diagnose problems with your process

#Why are you here?
- Learn how to solve problems well enough to keep a job as a software developer.
- teams look for those who:
  - solve problems effectively
  - learn new things quickly
  - get things done

#To Reiterate:

1. understand the problem
 - identify inputs and outputs
 - ask what if questions
2. Devise a solution
 - based on: your ability to execute it, performance, maintainabilty
3. Carry out the solution.
  - dispense with boilerplate code
  - write code outside in
4. Look back
  - check if you got the right answer
  - write output something like:
```
console.log("allManagers should be 0 and is", combinedExperience(allManagers));
```

If you've finished, that does not mean that you are done.
- burn and build when:
  - lots of typos/syntax errors
  - you struggled with the concept
  - you had to look things up
  - refactor when:
    - you finish early
    - you want to obtain multiple solutions
- write tests when:
  - the inputs and outputs feel smooth, and you are ready for more.
  - you want to speed up development process
- a great combo:
  - write tests
  - delete and rewrite solution
  - refactor
