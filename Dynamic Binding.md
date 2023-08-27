# Dynamic Binding

When the type of object is determined at runtime.

Happens when object of child is assigned to reference of parent.

Example:

```java
Human h = new Student()
//Student IS-A Human
```

```java
foo(Human h) //method definition

//method call
foo(Student s)
```

Reference of Human type ————>       Object of Student type.

(Reference Variable) ------------------>                                           (Object)

Argument —  [[Human h = new Student is not dynamic binding]]
