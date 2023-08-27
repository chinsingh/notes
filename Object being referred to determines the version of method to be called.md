# Object being referred to determines the version of method to be called

The object being referred to (not the reference variable) determines the version of method to be called.

So in this example, if Student has a method overriding a method in Human. Student's method will be called because even though h is an object of Human, it is referring to an object of Student.

```java
Human h = new Student();
h.overriddenMethod();
```

## References

[GFG - Dynamic Method Dispatch or Runtime Polymmorphism in Java](https://www.geeksforgeeks.org/dynamic-method-dispatch-runtime-polymorphism-java/)
