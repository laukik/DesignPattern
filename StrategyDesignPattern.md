Strategy Design Pattern
----------------------------
Not every problem can be solved by inheritance.
If we have set of Algorithms, allow algorithm to be plug and play.
Algorithm should be indipendent of the client and can be interchanged. 
Allow algorithm injection.

instead of providing method to be implemented by child, provide interfaces 
that can do it. So that Child can decide which behaviour it want dynamically.


```java

//Examples :
Interface ICommit{

    Interface:: ICommitMethod 
    Method :: doCommit();

}

Interface ICommitMethod {
    Method :: getMethod(); // Here Method can be OnePhaseCommit, TwoPhaseCommit, BatchCommit
}






