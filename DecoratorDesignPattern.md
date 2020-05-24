Decorator Design Pattern
-------------------------------
Providing behaviour dynamically.
Accomplished by Wrapping

Attached additional responsiblity to an Object and Runtime( Dynamically ).
Alternare option to subclassing for extending functionality.
//example :: Depricition

Interface IComponent{
    //Methods..
}

/***
*    IDecorator is a IComponent as well as has a IComponent
**/
InterFace IDecorator implements IComponent{
    InterFace IComponent;
    //Methods..
}