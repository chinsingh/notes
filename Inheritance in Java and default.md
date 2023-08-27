# [[Inheritance in Java]] and [[default]]

- Are [[default]] fields and methods inherited?

    Only if the subclass is located in the same package as the superclass.

- How is multiple inheritance handled in case of [[default]] methods?

    In case both parent interfaces have a default method with same method signature, the implementing class should explicitly tell which one its trying to use or it should override the default method.

    ```java
    //If I1 and I2 both have a fun() as default method
    class C implements I1, I2{
    I1.super.fun(); //Use I1's fun() method
    }
    ```
