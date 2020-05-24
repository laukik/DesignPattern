Decorator Design Pattern
-------------------------------
Providing behaviour dynamically.
Accomplished by Wrapping
Attached additional responsiblity to an Object and Runtime( Dynamically ).
Alternare option to subclassing for extending functionality.

```java
//example :: Depricition

interface IComponent{
    //Methods..
}

/***
*    IDecorator is a IComponent as well as has a IComponent
**/
interface IDecorator implements IComponent{
    interFace IComponent;
    //Methods..
}
