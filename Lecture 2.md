# Programming Methodology #2
#### Producer: [[Stanford University]] [[Mehran Sahami]]
#### Date: 2020-12-21
## Karel's Commands
1. move() -> move one step in it's direction
2. turnLeft() -> turns 90º counterclockwise
3. pickBeeper() -> picks up the beeper and put it in the beeper bag
4. putBeeper() -> take one beeper from the beeper bag and put in on the floor

## Turning Right as an Example
### 1. An Algorithm
A recipe for doing something.
```
turn left
turn left
turn left
```

### 2. A Piece of Code
```
turnLeft();
turnLeft();
turnLeft();
```

### 3. A Method
An instruction we can call.
```
private void turnRight() {
   turnLeft();
   turnLeft();
   turnLeft();
}
```

### 4. A Class
A class is a template of objects, where it encapsulates relevant behaviors and data of the objects.
```
public class ourKarelProgram extends Karel {
   public void run() {
      turnRight();
   }
   
   private void turnRight() {
      turnLeft();
      turnLeft();
      turnLeft();
   }
}
```
Note: Karel will run whatever is written in the `run()` method. In this case, it will `turnRight()`.

Note: In the Karel world, Karel must have a `run()` method in order to work. The `run()` method is an encapsulation of what Karel will be doing once the program runs.

### 5. A Complete Program
Something that is syntactically correct.
```
import stanford.karel.*;

public class ourKarelProgram extends Karel {
   public void run() {
      turnRight();
   }
   
   private void turnRight() {
      turnLeft();
      turnLeft();
      turnLeft();
   }
}
```
Note: since our class is based on the `Karel` class, it has to be imported from somewhere else, which is the `stanford.karel.*` library in this case.

## Loops and Conditionals
Until now, the program is rigid. It does not take in consideration about the situations.

No matter how you encapsulate the program, it will only solve one single problem. In order to make it solve different problems, you need loops and conditionals.

### 1. For Loops
This loop does the same thing as `turnRight()`.
```
for (int i = 0; i < 3; i++) {
   turnLeft();
}
```

### 2. While Loops
In this loop, Karel moves forward whenever the front is clear.
```
while (frontIsClear()) {
   move();
}
```

### 3. If Statement:
In an if statement, Karel executes instructions based on the conditions.
```
if (beeperIsPresent()) {
   pickBeeper();
} else {
   putBeeper();
}
```

### Nested Expression
You can put loops or conditionals within other loops and conditionals, as many as you need it. This is called a nested expression.

### Test Methods
Other than `beeperIsPresent()`, Karel has other test methods where you can check its states to determine the appropriate actions.

## SuperKarel
SuperKarel is an extended version of Karel, where it can `turnRight()`, `turnAround()`, paint, etc.
```
public class SuperKarel extends Karel {
   public void turnRight() {
      // code to make Karel turn right
   }
   
   public void turnAround() {
      // code to make Karel turn around
   }
   
   // other functionalities
   
}
```
![[Karel Commands.jpg]]