Command Design Pattern
---------------------------------
Allow Coomand request be created as an Object and parameterized it with set of command ,by which undoable opertions is also possible.
Removed the hard coding


Interface IInvoker{
    // Inject it, in the construtor.. 
    Set<ICommand> commands; 
    void invokeCommands();
}


//There can be Many Implementations  of this ICommand..
Interface ICommand{
    //Command has the Receiver on which it will be performed..
    IReceiver receiver;
    void execute();
    void undo();
}


Interface IReceiver{
    // Action to be Executed..
    void performCommand();
}
