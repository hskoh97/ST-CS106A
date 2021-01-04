# Programming Methodology #5
#### Producer: [[Stanford University]] [[Mehran Sahami]]
#### Date: 2021-1-2
## Variables
Variable is a box you can stick stuffs in and change it.

A typical variable has its name, type and value.

### Valid Variable Names
A valid Java name:
1. starts with a letter or an underscore;
2. can have any number of letters, numbers and underscores;
3. is not a reserved word.

### Primitive Java Types
1. int (integer)
2. double (real-value)
3. bool (boolean)
4. char (character)

#### The Distinction between an Integer and a Double
How much? vs how many? The distinction between discrete and countable values and continuous values is important.

### Declaring a Variable
Declaring a variable:
```
[type] [name];
```
e.g.
```
int x;
```

Declaring and assigning an initial value:
```
[type] [name] = [value];
```
e.g.
```
int x = 3;
```

Variables are always declared inside a method. These variables are always private to the method regardless of the public/private status of the method.

#### The '=' Operator
'=' is an assign operator, not an equality operator in a mathematical sense.
```
[variable] = [expression];
```

e.g. An increment:
```
total = total + 1;
```

#### The `+` Operator
`+` is an addition operator for both `int` and `double`.

`+` also works for `String`, it is a concatenation operator, connecting the latter `String` to the end of the former.

The notion of performing different functionality based on different data type is called overloading. In this case, the `+` operator is overloaded.

#### The `-` Operator
`-` is a subtraction operator when placed between two `int` or `double` variables.

`-` also works as a "negative sign" operator when it is placed in front of a `int` or `double` variable, it is technically called the "unary minus" operator.

#### Other Operators
`*` is a multiplication operator.

`/` is a division operator.

`%` is a remainder operator, it works like a modulo operator for positive integers, but also works for positive real numbers and negative real numbers. However, its behavior for negative real numbers does not make mathematical sense.

## Classes
### Initializing a Class
```
GLabel label = new GLabel("Hello world.", 100, 75);
```

`GLabel label` means that the variable `label` is initialized as a `GLabel` object.

`GLabel("Hello world.", 100, 75)` is a special method called a constructor. A constructor has the same name as the class and is used to create a new object based on the class.

A constructor is a 'factory' that produces new objects.

### Manipulating an Object
When an object is initialized, you can tell it to do something by calling its methods.

As `GLabel` has methods such as `setFont()` and `setColor()`, you can call these methods to change its font and color.

Make a method call on an object:
```
label.setFont("SansSerif-36");
label.setColor("Color.RED");
```

in these commands, label is the "receiver" of the method, while `setFont()` and `setColor()` are the "messages" sent.

#### About the ACM Canvas
If you have called the `add()` method, the canvas will change immediately once you change the properties of the objects displayed.

### GObject Methods
```
setColor([color]);
setLocation(x, y);
move(dx, dy);
```

The `color`s are defined in the Java Color Library (`java.awt`).
```
Color.BLACK
Color.CYAN
Color.LIGHT_GRAY
etc.
```

#### GLabel Specific Methods
```
setFont([font])
```

The `font`s are defined as below:
```
family-style-size
```

Where the `style`s available are defined as below:
```
PLAIN
BOLD
ITALIC
BOLDITALIC
```

#### Geometrical Shapes
`GRect`:
```
new GRect(x, y, width, height);
setFilled(fill) = [bool];
setFillColor([color]);
```

`GOval`:
```
new GOval(x, y, width, height);
setFilled(fill) = [bool];
setFillColor([color]);
```

`GLine`:
```
new GLine(x0, y0, x1, y1);
```

`GraphicsProgram`:
```
getWidth();
getHeight();
```

