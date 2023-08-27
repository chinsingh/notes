# Suffixing for Non-default Primitive Data Types

## `int` and `long`

Default type for integer literals is `int`. That is, unless specified otherwise, 35 is an `int`. So if we assign an integer directly to a `long` variable, it will result in compilation error.

```java
//Compilation error
long x = 232342;
```

Thus, we have to specify explicitly that the value 232342 is a `long`.

This can be done by suffixing `l` or `L` to the value. For example. `232342L`.

## `float` and `double`

Similarly, double is the default value for floating point literals. Unless explicitly stated, 9.5 is a `double` not a `float`.

```java
float a = 3.7 // 3.7 is a double, ‘a’ is float => Error
float a = 3.7f // a is a float
```
