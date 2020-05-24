Abstract Factory Design Pattern
-------------------------------------
It is a set of Factory Method Design Pattern
Provides interface for creating  families of related or dependentObject without specifiying the name of its concrete implementation
```java
//example :: Create UI Control for diffrent OS.
Interface IComponent{
    //Methods
}

Interface IComponentX implements IComponent {
    //Methods
}

Interface IComponentY implements IComponent{
    //Methods
}

Interface IComponentFactory{
    IComponent createX()
    IComponent createY()
    //...
}
