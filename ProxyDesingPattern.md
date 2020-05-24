Proxy Desing Pattern
------------------------------
It provides a placeholder for another Object in order to control access to it.
//May seem same as Decorator but the both have diffrent reasons.
// unlike Decorator it is not adding behaviours.. 
Types 
Remote      :: Used for Remote Resources
Virtual     :: Control access to a Resource that is Expensive to create  // can do lazy implemetation example :: Book Parser, Cache
Protection  :: Used for Access Management , control a Resource based on Access type

interface IClient{
    // Instead of Component we will have the proxy for same..
    IComponent proxyComponent;
}

interface IComponent{
    //Methods..
}

class ConcreateComponent implements IComponent{
    //Methods
}


interface IProxyComponent implements IComponent{
    IComponent concreteComponent;
    // All methods implementation will be done and call will be made to concrete Component.. 
}

