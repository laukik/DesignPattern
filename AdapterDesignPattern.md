Adapter Design Pattern
--------------------------------
Also known as wrapper
it allows two interfaces to get compitable with each other.
it converts ome interface to another interface that client expect.
//example : Universal Power Adapter..

//  It Allow us to keep the implementation of the ITarget same
//  And based on calling IClient, we inject the IAdaptee

interface IClient{
    ITarget target;
    void doAction(); // calls target.action()
} 


interface ITarget{
    void action(); // calls adaptee.convertReuqest() to create ITarget type input;
}


class Target implements ITarget{
    IAdaptee adaptee;
    void action(); // calls adaptee.convertReuqest() to create ITarget type input;
}

interface IAdaptee{
    convertReuqest(); // Handles the Request and support the Compatiblity..
}


