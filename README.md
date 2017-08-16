# Application Logic

## Pseudocode

- Oftentimes in applications you will be solving problems that you have never solved before and are not sure how to do.
- Pseudocode is a technique for tackling these problems without writing real code in an effort to understand the mechanics behind what has to happen programmatically.

## What does that look like?

Pseudocode should describe the entire logic of the algorithm so that programming becomes a task of translating lines of pseudocode into real code.

For each of the following, let's discuss why each pseudocode could be considered "Good" or "Poor" examples of pseudocode:

#### Problem 1 - Determining If a Number is Even or Odd

***Example 1.1:***

```
PROGRAM IsEvenOrOdd:
  var num = number;
  IF (num % 2 === 0)
    THEN Print "even";
    ELSE Print "odd";
  ENDIF;
END.
```

***Q. What do we think?***

> A. This is not a great example. Here we are using "var" in our pseudocode when it should read plain english! Also, we should not be using the javascript syntax "===" in our conditional.  Would a non-programmer know that `num % 2 === 0` indicates an even number?

***Example 1.2:***

```
PROGRAM IsEvenOrOdd:
  Read number;
  IF (number divided by two has no remainder)
      THEN Print the number is even;
      ELSE Print the number is odd;
  ENDIF;
END.
```

***Q. What do we think?***

> A. This is better.  It's closer to english.  It clearly states what we are trying to achieve and how, without getting bogged down in the minutia of code.  Even someone that doesn't code can help us check our logic.  Is any number that can be divided by two, cleanly -- without leaving a remainder -- even? Is anything else odd?

#### Problem 2 - How to Make a PB&J Sandwich

*From [Get Creative Today](http://getcreativetoday.com/lessons/pseudo-code-flowcharts/)*

***Example 2.1:***

```
Make PB&J Sandwich:
  Gather bread, peanut butter and jelly.
  Apply peanut butter to slice of bread.
  Apply jelly to another slice of bread.
  Bring the two slices of bread together.
  Eat and enjoy.

```

***Q. What do we think?***

> A. This is a good place to start.  It is a good set of instructions and intuitive for us to follow.  However, we still don't know what physical steps are required.

Take a second to imagine.  Imagine if you had never made a sandwich before.  Ever.  Think about the instructions you would need for that first sandwich.  A computer has no real memory.  Every time it starts a task, it has no recollection of performing it before.  We must tell it every single step, every single time.  We need to break these down into smaller steps for the computer to understand.

***Example 2.2:***

```
PROGRAM MakePB&JSandwich:
  Grab a paper plate;
  Open bread container;
  Grab bread package;
  Untwist bread package;
  Open bread bag and remove two slices;
  Place slices on paper plate;
  Grab a plastic knife;
  Open peanut butter jar;
  Use knife to scoop out peanut butter;
  Apply peanut butter to one slice of bread;
  Spread peanut butter on slice;
  Place knife on plate;
  Close peanut butter jar;
  Open jelly bottle;
  Squeeze jelly onto second bread slice;
  Close jelly bottle;
  Place down jelly;
  Pick up knife;
  Spread jelly on slice;
  Bring two slices of bread together;
  Cut slices in half down the middle;
  Throw knife in the trash;
  Pick up one half of sandwich;
  Enjoy;
END.  
```

****Q. What do we think?****

> A. This example's sequence is very thorough! However, we are still assuming certain conditions that our utensils or ingredients already exist. What if we are out of plates? Will we grab a napkin instead to place our sandwich on? What if we are out of jelly? Will you throw the sandwich away or eat it with just peanut butter?

Computers are not smart. We need to give them step-by-step instructions to account for conditions. They can not adapt to make changes without being explicitly told. Programming is a series of tasks, which can be completed only if a certain number of conditions are met.

Computers can not adapt, but we can.  Your first pass at pseudocode will probably not cover everything.  Once you know more, you may come back to update and refactor your pseudocode.

***

## Approaching a coding problem

Pseudocode isn't just about writing down the steps that you already know.  It's a tool to help you work through the problem.  Before we can write pseudocode to solve the problem, we need to know the problem.  

Here are some steps that can help with problem solving:

- Identify the Problem
- Conceptualize
- Break it down
- Start small

#### Identify the Problem

- What exactly are we trying to solve?  - From who's viewpoint?  
- Who will benefit?  
- What are we delivering?

#### Conceptualize

- Look at the big picture, the major steps
- Avoid details
- At this stage we recommend drawing on whiteboards or with pen and paper, anything that screams "temporary", "play", or "brainstorm".

#### Break it down

- We break the conceptual models down into concrete steps, actionable items.
- We identify risks (gaps in knowledge, technology, and infrastructure).

#### Start small, stay small

Finally, we take some action. This is when we finally start writing code. We fight hard to take small steps, verify that each step achieves what we want, what we expect, before continuing on. If we do too much at once and things break, which they always do, we won't know what is causing the problem. We won't know which part to trust. Humans thrive on easy wins. We need to see forward progress. Remember that.  Use that. Celebrate your wins.


#### Review: the Steps

- Identify the Problem
- Conceptualize
- Break it down
- Start small


****Q. Where does pseudocode fit in these steps?****

> A. Break it down OR Start small

This process is iterative.  We keep circling around and repeating the earlier steps, just at a different level.

When we first approach a problem, we see the big picture.  "Break it down" gives us big steps.  Then, we take one of those steps and "Break it down".  Now, starting small, we write pseudocode to help illustrate the problem.  

Pseudocoding proves that we have *identified* the problem, understand it *conceptually*, and have *broken it down* into *small steps* that we can follow.


#### Syntax for Pseudocode:

There is no one, fixed syntax for pseudocode.  It just needs to be clear, simple, and concise.  

If you feel stuck, feel free to use this syntax:

***Referencing: [Introduction to Pseudocode](http://www.slideshare.net/DamianGordon1/pseudocode-10373156)***

* General Structure of Pseudocode

	```text
	PROGRAM <ProgramName>:

	<Do Stuff>

	END.
	```

* Selection: IF/ELSE Statements

	```
	IF (<Condition>)
		THEN <Statements>;
		ELSE <Statements>;
	ENDIF;

	```
* Iteration: LOOP

	```
	WHILE (<Condition>)

	ENDWHILE;
	```

***
<a name="real-world-practice"></a>
## Independent Practice: Pseudocode a real-world problem (15 min)
Follow the instructions in [starter\_code/pseudo\_code\_practice.md](starter_code/pseudo_code_practice.md)

## Extra Work: Bubble Sort

- [Explanation on how it works](https://www.tutorialspoint.com/data_structures_algorithms/bubble_sort_algorithm.htm)
- How can we design pseudocode to accomplish this algorithm?
- Now that we understand how to do this with numbers, how could we design a similar algorithm to do it with letters?

### ADDITIONAL RESOURCES

- [Pseudocode](https://en.wikipedia.org/wiki/Pseudocode) (Wikipedia)
- [Introduction to Pseudocode](http://www.slideshare.net/DamianGordon1/pseudocode-10373156)
- [Get Creative Today](http://getcreativetoday.com/lessons/pseudo-code-flowcharts/)
- Videos
	- [Matt, WDI-DC-8 Screencast](https://www.youtube.com/playlist?list=PL-6bwUTtCRVTMUUSjqIYVXYyfZBzs8saD)
	- [GA JS Circuit - Pseudocode](https://generalassembly.wistia.com/medias/ym3vdun7n3)
