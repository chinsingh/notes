# Creating Objects in Java

```java
Box smallBox;
```

- Unlike [[Creating Objects in C++]], the above statement won’t create an object. It will just create a reference variable. The reference variable has to be given an object.

```java
Box smallBox= new Box();
```

Now `smallBox` contains address of an object of Box class. That is, it points to the object. However, the object itself has no name.
