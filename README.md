Download Link: https://assignmentchef.com/product/solved-cs314-programming-assignment-5
<br>
<h1 class="product-top-header" title="CS314 Programming Assignment 5 Solved"><span style="font-size: 16px;">The purpose of this assignment is to implement a linked list class that uses doubly linked nodes. Doubly linked nodes have references (pointers) to the next node in the list and back to the previous node in the list. This makes some things harder because there are more references (pointers) to set up. But, it makes a lot of things easier because it is possible to back up in the list without having to start over at the beginning, use the look ahead technique, or use a trailer node.</span></h1>

5/5 - (2 votes)

Files:

FileResponsibilitySource CodeDoubleListNode.java (Alternatively you make this a static nested class to the LinkedList class for the doubly linked nodes as demonstrated in lecture. None of the test cases reference the DoubleListNode class.)Provided by me. Do not alter the stand alone class.Source CodeIList.java Interface your LinkedList class implements.Provided by me. Do not alterSource CodeStopwatch.javaProvided by me. Do not alter.ImplementationLinkedList.java. Implementation of a doubly linked list.Provided by you and me.  (Okay, mostly you.)Test codeLinkedListTester.java. Test harness. correct any tests that have errors. Ensure your LinkedList class passes the tests included and add more tests.Provided by you and me.Optional Visual TesterLinkedListView.java An tool [its use is optional] created by one of our TAs [Andrew] for viewing the LinkedList. Refer to the documentation on the GitHub page. The class can be downloaded there.Provided by me (Okay, TA Andrew)DocumentationJavadoc files for DoubleListNode and IList.

Draw pictures!! When completing methods and figuring out all the references that have to be updated and what the special cases are DRAW PICTURES of the linked structure. This is much easier than just looking at code and trying to figure out what must be done or why something does not work.

Please realize, when you get an error in a test the cause is typically in another method. It is often the case that students make errors when adding or removing elements or changing the structure of the internal storage container (the linked structure of nodes), but the error does not show up until later on a test of toString.

Implementation details:

Complete the LinkedList class.  For this assignment you may not use the LinkedList or ArrayList classes from the Java standard library. You must implement the underlying storage container as a doubly linked structure using the DoubleListNode class. The DoubleListNodes and LinkedList are generic based on Java’s generic syntax.

You may approach the implementation in many ways. (References to first and last node, circular list with only a link to the first node, use of header nodes that don’t contain any data) The approach you take is up to you. Each has certain advantages and disadvantages.

In addition to implementing the methods specified in the IList interface you must add  the following methods to the LinkedList class. E is the data type variable. It will hold what the data type is for the elements (thus the E) of a particular LinkedList object.

void addFirst(E item) // add an item to the front of this LinkedListvoid addLast(E item) // add an item to the end of this LinkedListE removeFirst() // remove the first item in this LinkedListE removeLast() // remove the first item in this LinkedListoverride the toString method. The data in the list should be listed between square brackets with a comma between each item and a single space after each comma. e.g. [A, B, C]public String toString()override the equals method. Two ILists are equal if they have the same number of elements in the same order.public boolean equals(Object other). Two empty lists are equal regardless of the kinds of elements they store. (This is true in the Java standard library.) Also note, we are implementing the IList interface. To meet the requirement IList puts on classes that implement it, your LinkedList is considered equal to any other IList (not just a LinkedList) if it has the same elements in the same order.LinkedListTester provides some tests for the LinkedList class. Some of these tests may be incorrect. Find and fix any incorrect tests. Your class must pass these (corrected) tests. In your final submission delete the provided tests. Add at least 3 tests of your own per method in the LinkedList class to the LinkedListTester class. Delete the provided tests. You may post the tests you write to the class class discussion group, but in the end you must implement your own tests.

Note, most of my tests rely on your iterator method. If that is not working you will fail those tests. I strongly recommend you test your methods as you complete them by writing your own tests! Write a method, then test it. Write a method, then test it. DON’T do this:  write a method, write a method, write a method, … then test …then debug, debug, debug, debug, debug, debug, debug, debug, debug, debug, debug, debug.

For every method in the LinkedList class state the Big O of the method if there are already N items in the list.

The methods for the iterator for your linked list shall all be O(1).  You shall replace the default remove method from the Iterator interface with a remove method that actually removes the last element returned by next. Your iterator class does NOT need to detect co-modification errors.

If a method has preconditions you must check those preconditions and throw an Exception if they are not met.

You can, of course, implement methods using other methods from the class. You should only do this if the version of a method that relies on other methods in the class is as efficient as not using other methods.

As always, use good style: comments for non obvious algorithms and operations, good variable names, use helper methods if necessary, make operations as efficient as possible given the constraints.

Experiments: It is interesting and important to know the difference in behavior between linked lists and array based lists. When your LinkedList class is finished, run the comparison method from the LinkedListTester class which performs a number of tests with your LinkedList and the Java ArrayList class. To run the method simply uncomment the line at the end of the main method in LinkedListTester that calls the comparison method. You are free to change the initial value of N for the various tests in the comparison method.

In a comment at the top of your LinkedListTester class indicate which operations are faster when using your LinkedList, which are faster when using the Java ArrayList class, and which ones are about the same.  (Realize the experiments use different starting values of N.)

For the operations tested via the experiment what do you think the Big O of each operation / method is based on the timing data? State your reasoning.

Submission: Fill in the header in the LinkedListTester.java and LinkedList.java files.. Replace &lt;NAME with your name. Note, you are stating, on your honor, that you did the assignment on your own.

Create a zip file name a5.zip with your LinkedListTester.java and LinkedList.java files. The zip file must not contain any directory structure, just the required files.

See this page for instructions on how to create a zip via Eclipse.

Turn in a5.zip via your Canvas account to programming assignment 5.