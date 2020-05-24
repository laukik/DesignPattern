Observer Design Pattern
------------------------------
Notion is to remove polling.
it is Push intstead of Poll


Publisher           Subscribers
        "notify"
+++++                +++++
+ P + -------------> + S +
+++++                +++++

1. Observers needs to register themselves to the Subject(Publisher).
2. In case of state change Subject will notify all the Observers

interface ISubject{
    IObserver[]
    addObserver(IObserver)
    removeObserver(IObserver)

    // for each Observer in IObserver[] do :: Observer.execute();
    notify()
    
}

interface IObserver{
    ISubject // In Order to figure out what was Changed, we need Subject Refrence
    execute()
}