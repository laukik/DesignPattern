Abstract Factory Design Pattern
-------------------------------------
It is a set of Factory Method Design Pattern
Provides interface for creating  families of related or dependentObject without specifiying the name of its concrete implementation
```java
//example :: Create UI Control for diffrent OS.
interface IComponent{
    //Methods
}

interface IComponentX implements IComponent {
    //Methods
}

interface IComponentY implements IComponent{
    //Methods
}

interface IComponentFactory{
    IComponent createX()
    IComponent createY()
    //...
}
