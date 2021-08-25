This is my summary of the Introduction to Algorithms (CLRS).

Contributions: Issues, comments and pull requests are super welcome 😃

<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->
# Table of Contents
- [Table of Contents](#table-of-contents)
- [Chapter 1. The Role of Algorithms in Computing](#Chapter-1-The-Role-of-Algorithms-in-Computing)
- [Chapter 2. Gertting Started](#Chapter-2-Getting-Started)
<!-- /TOC -->

# Chapter 1. The Role of Algorithms in Computing
 - Algorithm can be defined informally as an well-defined computational procedure that takes some value, or set of values, as input and produces some value, or set of values, as output.
 - The statement of a computaional problem specifies in general terms the desired I/O relationship.
 - An instance of a problem consists of the input needed to compute a solution to the problem.
 - A correct algorithm should halt with correct values of every input instance.
 - Incorrect algorithm is also useful if we could control the error rate.
 - An algorithm can be specified in English, as a computer program, or even as a hardware design.
 - The only requirement is that the specification must provide a precise description of the computational procedure to be followed.
 
# Chapter 2. Getting Started
Insertion sort works the way many people sort a hand of playing cards. We start with an empty left hand and the cards face down on the table. We then remove one card at a time from the table and insert it into the correct position in the left hand. To find the correct position for a card, we compare it with each of the cards already in the hand, from right to left.  At all times, the cards held in the left hand are sorted, and these cards
were originally the top cards of the pile on the table.

    INSERTION-SORT(A)
    for j = 2 to A.length
    	key = A[j]
    	i = j - 1
    	while i > 0 and A[i] > key
    		A[i+1] = A[i]
    		i = i - 1
    	A[i+1] = key

 - Loop invariants help us to understand why the algorithms is correct.
 - The 3 properties of a loop invariant:
	 - Initialization: It is true prior to the first iteration of the loop.
	 - Maintenance: If it is true before an iteration of the loop, it remains true before the next iteration.
	 - Termination: When the loop terminates, the invariant gives us a useful property that helps show that the algorithm is correct.
 - There is a similarity between mathematical induction and loop invariant.
 - Showing that the invariant holds before the first iteration corresponds to the base case, and showing that the invariant holds from iteration to iteration corresponds to the inductive step.

