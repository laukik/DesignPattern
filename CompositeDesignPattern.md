Composite Design Pattern
---------------------------------
It Allow an Object as well as a Composite Object to be treated in uniformly.
Arrange the Objects into tree structure.

```java
// Example Tree : We need all the nodes i.e. root, intermidiate as well as Leaf Nodes to be treated in exact same way.
// React/Redux Framework uses Composite Pattern.
// 

interface Component{
  //Set of Methods..
}

interface CompositeComponent implements Component{
  set<Component> components;
}

interface SingleComponent implements Component{
  //Methods..
}
