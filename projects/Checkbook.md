---
layout: project
type: project
image: images/LinkedListIcon.PNG
title: Checkbook
permalink: projects/checkbook
# All dates must be YYYY-MM-DD format!
date: 2019-01-26
labels:
  - Linked List
  - Programming
  - C
summary: I learned about using linked lists and created a program to prove it.
---

<img class="ui medium right floated rounded image" src="../images/checkbook.jpg">

One of the projects that I took on during my ICS 212 class, was to utilize a linked list and writing the code in C.  Linked lists are data structures that have objects (nodes) that “link” together through pointers that reference to the next object.  Part of this project was to write a program that would create a check, delete a check, display a specific check, and display an entire checkbook. Some of the added variables to make it more interesting, was to specify functions to search by check number, amount formatting to two decimal places, and to display the proposed check input before adding it to the check book.

Being a novice programmer, I found difficulty in translating what I wanted my pseudocode to do in C.  I approached the problem with one segment at a time and ensured those segments worked.  The function calls gave me the most resistance, but through persistence and careful review of my class notes, I was proud of the product output.  This project provided a deeper understanding of programming in C as well as a practical application of linked lists.


Here is some code that illustrates how I displayed the found check:

```js

{
// Display the found node information

    printf("\n Check Number: %d \n Date: %s \n Given To: %s \n Check Amount: %.2f \n Check details: %s",
      currentNode->checkNumber, currentNode->date, currentNode->to,
      currentNode->amount, currentNode->description);
}
```
