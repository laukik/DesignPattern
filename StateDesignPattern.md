State Design Pattern
--------------------------
Behaviour of the Object will depend on the state, not on the Path through which they reach the state.
And based on current state it can change the behaviour at runtime.

```java

interface State{
  void handle();  // Behaviour that can be implemented by diffrent concrete classes depedning upon the possible state 
}

interface Context{
  State state; // Context at any point knows it's state, and delegate the action to the state handler..
  void request(); // Calls state.handle() in implemenataion
}

