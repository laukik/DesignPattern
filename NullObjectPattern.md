Null Object Pattern
---------------------------
Instead of introducing conditional for the Null check, just provide a child that does the implementation for the Null Object.
It reduce conditionals.
Allow us to treat Null Objects same as general Objects.

```java
// Examples :: Iterator interface in java also has EmptyIterator
// Composite Design Pattern goes hand in hand with Null Object Pattern

interface Iterator{
  //Some Method..
}

class EmptyIterator implements Iterator{
  // Some implemenation for that case when the Collection is Empty
  // So that we don't need any check everytime for if iterator is null..
}
