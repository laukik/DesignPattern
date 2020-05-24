Factory Method Design Pattern
-----------------------------
Uniforms object creation
Allows Creation of Object based on Business Logic
Define an interface for creating an Object but let the SubClasses decide what will be instantiated
```java
interface IComponent {
    //Methods..
}

interface ComponentFactory {
    //Returns Concrete implemenetion of IComponent
    //Based on Given input
    IComponent createComponent();
} 
