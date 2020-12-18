# Programming Methodology #3
## Good Programming Practices
While computers are ultimately the one reading your code, it can be written like English.

While a program can work even if human can barely understand it, it is hard to make changes in the future. Good programming practices make it easier for people to maintain programs and add new functionalities.

> Programming is not just about writing programs where computers understand, it's about writing programs where people understand. – Mehran Sahami >

### Comments
A good program should have comments. Comments are commonly used in
- describing the functionalities of a program
- describing code that are not obvious
- describing pre-conditions and post-conditions of a method

#### Describing the Functionalities of a Program


#### Describing Pre- and Post-conditions of a Method


#### Single-line Comment
Single-line comment ends when there is a line break.
```
// This comment ends here.

public void otherFunction() {
   
}
```

#### Multi-line Comment
Multi-line comments start with a `/*` and end with a `*/`, they are usually stylized every line.
```
/* This is a
 * multi-line
 * comment.
*/
```

### A Top-Down Approach to Programming: Decomposition
A top-down approach to programming is to solve problem starting from the highest level of abstraction, decompose high-level methods into low-level methods and eventually into primitives.

Primitives are instructions which the program already know: e.g. `turnLeft()` and `move()` are primitives to the `Karel` class.

You have to be comfortable to invent non-existent methods before defining them. The goal of top-down approach is to have a **well-defined compartmentalization of functionalities**.

#### The Bottom-Up Approach
The bottom-up approach solve problems using primitives directly.

It can be intuitive to using the bottom-up approach, but as problems get bigger and more complex, this approach will be much harder to maintain.

#### Top-Down Approach Examples


### Good Practices in Writing Methods
Rules of Thumb? A typical method should
- basically solve one problem (at that level of abstraction).
- be around 1-15 lines long.
	- Single-line method? Single-line method gives the underlying method a new purpose: it renames the method.
- have good names
	- CamelCase
	- firstLetterSmallCamelCase
	- underscored_name
	- may refer to Python PEP naming conventions
- have comments
	- state their functions
	- state their pre-conditions
	- state their post-conditions

## Common Errors
### Infinite Loop


### Off-by-One-Bug (OBOB)