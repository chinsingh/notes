# [[Runtime Polymorphism or Dynamic Method Dispatch]] -- When you override - you get it -- when you hide - you don't

```java
class Foo {
    public static void classMethod() {
        System.out.println("classMethod() in Foo");
    }
 
    public void instanceMethod() {
        System.out.println("instanceMethod() in Foo");
    }
}
 
class Bar extends Foo {
    public static void classMethod() {
        System.out.println("classMethod() in Bar");
    }
 
    public void instanceMethod() {
        System.out.println("instanceMethod() in Bar");
    }
}
  
public class Test {
    public static void main(String[] args) {
        Foo f = new Bar();
        f.instanceMethod();
        f.classMethod(); //*Accessing static method using object
    }
}
```

Output -

```java
instanceMethod() in Bar
classMethod() in Foo
```

We are using the same instance to access both the methods. But since one is overriding and the other is hiding, we see different behaviours.

- In case of instance method-

    At runtime, JVM uses the instance 'f' to determine which method to run.

    JVM sees at runtime, that 'f' is actually an instance of Bar, so it calls the method in Bar rather than the one in Foo.

- In case of class (static) method-

    Since, its a static method, JVM doesn't expect or need any instance to invoke that method. Even if you provide it with an instance like we did here, it will simply ignore it. It will just see the declaration of that instance, determine the declared type of it to determine which method to call. All of this, at compile-time.

    It doesn't matter when at runtime, its decided that f is actually an instance of Bar. That's what we mean when we say a static method does not have run-time polymorphism.

    Because of this difference in behaviour in static and instance methods, we use different terms - "overriding" for instance methods and "hiding" for class methods.

    And when we say, you can't override a static method, it means you can write the code that looks like a static method being overridden, but it won't behave like an overridden method.

*Notice that [[Accessing Static members using objects]] is possible
