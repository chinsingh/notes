# String Memory Management

## String Initialization using literals

Creating a String literal → JVM checks the [[String Constant Pool]]
  
- Exists => Points to the same 'literal'
- Doesn't Exist => New instance created

## String Initialization using new

```java
String str = new String(); //null
String str = new String("Kya challa?")
```

New object created irrespective of whether the literal already exists or not
