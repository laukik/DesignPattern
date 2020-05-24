Template Method Pattern
-------------------------------
It defines skeletion of an algorithm for an operation deefering some steps to the subclasses, And allow subclasses to defeine the algorithm without changing the inner implementation.
Hooks are the ways to achieve the same.
One way to implement Open Close Principle.

```java
/**
* example :: Frameworks
*/

abstract class AbstarctClass{
  
  templateMethod(){
    //Method which has generic Code..
    //Some Implementation...
    hookMethod();
    //Some More Code...
  }
  hookMethod();
}

class ConcreteClass extends AbstarctClass{
  hookMethod(){
    //Implementation that Sub Classes Define..
  }
}
