# [[Static]] in Java

## Example of class containing static members

```java
public class Example
{
int x; // Instance variable
static int y; // Static member variable

public void fun() { static int a; } // Instance member function
public static void fun2() { } // Static member function 

static class Test //Static inner class
{ }
}
```

## [[Static Variable]]s

- Initialization

    Values can be assigned in special static initializer blocks / [[static Blocks]]

- Accessing

    Accessing outside class - `ClassName.VariableName`

- Naming

    When declaring class variables as public static final, then variable names (constants) are all in upper case. If the static variables are not final, the naming syntax is the same as instance and local variables.

## [[Static Blocks]]

## [[Static Method]]s

## Static class

[[Static Inner Class]]
