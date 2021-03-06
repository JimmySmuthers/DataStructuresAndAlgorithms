# DataStructuresAndAlgorithms
UC3M, Y1Q2

Programming language: Java

Exercises done in the Data Structures and Algorithms class. This README will contain a brief explanation of every exercise.



Exercise 4: SList implementation.

  Here, we create the single-linked list data structure, composed of the following:
    
    Interfaces
      IList.java
      
    Classes
      SNode.java
      SList.java
      SListCircular.java
      SListTail.java
      Test.java
      SListInteger.java (Exercise 6)
      
  Single-linked lists are managed using nodes. These type of lists have a fixed firstNode, which will be the starting point for every other node needed. Every element in the list is retrieved, created or deleted using nodes. Nodes are objects which contain a generic type element, and have a nextNode attribute which points to the following node. This pointer is what allows us to modify the list. A node that points to null is the last element in the list (not the case for circular lists), and a node that is not pointed to by any other node is deleted from the list, as there is no way to access said node. 
  
  Circular lists do not contain a node that points to null. This last element will simply point to the first element.
  
  Tail lists store the first node and the last node of the list.



Exercise 6: SListInteger 

This file is contained in the Exercise 4 folder, given that it needs the SList class to function.

  Implementation of the SListInteger class that extendes the SList class. In it are included methods used to calculate the sum of all the numbers in the list and another which will return the even numbers of the list.



Exercise 7: DList implementation
  
  Here, we create the double-linked list data structure, composed of the following:
  
    Interfaces
      IList.java
      
    Classes
      DNode.java
      DList.java
      Palindrome.java (Exercise 8)
      
  Double-linked lists work the same way as single-linked lists, the only differences are that each node now has two pointers, a PREVIOUS pointer and a NEXT pointer, and it also contains two special nodes called sentinel nodes.
  This list contains two sentinel nodes, the HEADER node and the TRAILER node. These nodes do not contain any elements, their only content is null. The HEADER node sits in position -1 of the list (at least for this implementation) and is the first node of the list. Its PREVIOUS node points to the TRAILER and its NEXT node points to the first element-containing node of the list. Likewise, the TRAILER node is the last node of the list; it's PREVIOUS node points to the last element-containing node and it's NEXT node points to the HEADER.
  The only purpose of these sentinel nodes is to have a sense of direction regarding the first and last elements of the list.



Exercise 8: Palindrome

  This file is contained in the Exercise 7 folder, given that it needs to use the DList.java class in order to function.
  
  This class checks if the specified word is a palindrome, i.e.: if it is read the same backward as it is forward. For example: racecar.
  


Exercise 9: Operation Balancer using Stacks

  Here, we create the class Expression and are supposed to be able to tell whether this mathematical operation is properly written in terms of grouping symbols. What this means is that every opening parenthesis, bracket, or curly bracket must have its closing counterpart in the correct order. For instance: ({1+3)} is not correct. However, ({1+3}) is. 


Exercise 10: Mixing	ordered	queues

  We are supposed to write a java program that is able to receive as parameters two single queue objects and return only one single queue, which must be ordered. To add a bit more of complexity to the problem, we assume that these two queues received as parameters are not ordered. This can probably be vastly optimized, without having to create so many auxiliary variables in the mixer method.
  

Exercise 11: Company ArrayList

  We are supposed to create two classes, the Employee class and the Company class. Using methods belonging to the ArrayList class, we are to create some new methods for the Company class.
