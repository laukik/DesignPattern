Facade Design Pattern
-------------------------------
It provides unified interface for a set of interfaces  in the subsystem.
It defines an higer level interface.
Helpful when many classes are interdependent and using eah other.
//example : Compiler 
//Principle of least knowledge { Law of Demeter}

interface IClient{
    IFacade facade;
}

interface IFacade{
    //Methods to call classes it is Facade for..
    void doSomethingIA();
    void doSomethingIB();
//  ..
//  ..
    void doSomethingIZ();
}


// here A, B ...Z are using each other
interface IA{
    
}

interface IB{
    
}

...

interface IZ{
    
}


