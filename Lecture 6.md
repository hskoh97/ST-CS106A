# Programming Methodology #6
## Receiving User Input
```
int x = readInt("");
double y = readDouble("");
```

## Mathematical Operations
### Division of Integers
Integer divisions yield integer numbers, thus the remainder is discarded in an integer division.
```
5/2 = 2; // remainder 1 is discarded
5/2.0 = 2.5 // double division
```

In this case, even if `y` is a `double`. The expression is an `int`, therefore the truncated answer is assigned to `y`.
```
int x = 5;
double y = x/2; // y = 2.0 != 2.5
```

### Operator Order of Precedence:
1. parentheses
2. multiplication, division and remainder
3. addition and subtraction

```
int x;
x = 1 + 3 * 5 / 2 // x = 8
```

Java does not have primitive exponent operator.

### Type CAST
In order to solve the integer division problem while retaining the `int` data type, type cast is used:
```
int x = 5;
double y = (double) x/2; // y = 2.5
```

In this case, the expression `x/2` is cast into a `double` and the evaluation is assigned to `y`. Note that `x` remains an `int`.

You can also assign a `double` to an `int` using type cast.
```
double y = 2.5;
int z = (int) y; // 2, truncated, not rounded up
```

Actually, you do not need to cast `y` into an `int`, this type conversion is automatic. The above example shows the purpose of a type cast only.
```
double y = 2.5;
int z = y;
```

#### Calculating an Average of Two `int`s
```
int n1, n2;
n1 = readInt("First number:");
n2 = readInt("Second number:");

double avg = (double) (n1 + n2)/2.0
```

#### Formatting the Display of Numbers in Java

### Frequently Used Shorthands
#### Increments/Decrements
```
int x = 1;
x = x + 1;

int y = 1;
y = y - 1;
```

```
int x = 1;
x += 1;

int y = 1;
y -= 1;
```

```
int x = 1;
x++;

int y = 1;
y--;
```

#### Multiplications and Divisions
Multiplication:
```
int x = 2;
x *= 2;
```

Division:
```
int x = 2;
x /= 2;
```

## Constants
Constant serves the purpose of an immutable value. While variables can also serve the purpose of a constant, constants guarantees the immutability of the value and retains data integrity.

```
double PI = 3.1415926535; // This value can be changed below with just an assignment.
```

Defining a constant:
```
private static final double PI = 3.1415926535;
```

### Naming Conventions of a Constant
1. All capital letters
2. Readable name

### Java Math Library
Most mathematical constants have been defined and can be found in the Java Math Library.