Singleton Design Pattern
--------------------------------
Allows only one instance of the Object to be created and make it available globally via a single contact


class Singleton{
    private Singleton();
    static Singleton inst;
    static Singleton getInstance()
}

