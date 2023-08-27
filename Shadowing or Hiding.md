# Shadowing or Hiding

- **Overriding** => In case of non-static methods

    ```java
    class A{
        public void show(){
        System.out.println("in A");
        }
    }

    class B extends A{
        public void show(){
        System.out.println("in B");
        }
    }
    ```

- **Hiding** => In case of all other members (instance members, static members, static methods)

    ```java
    class A{
    int a;
    static int b;
    static meth();
    }

    class B extends A{
    int a;
    static int b;
    static meth();
    }

    //class B now has both properties.
    //'a' from its own class
    ```

## Major Difference between [[Method Overriding]] and Hiding

This

```java
class Foo {
    public void method() {
        System.out.println("in Foo");
    }
}
 
class Bar extends Foo {
    public void method() {
        System.out.println("in Bar");
    }
}
```

is not the same as this

```java
class Foo {
    public static void method() {
        System.out.println("in Foo");
    }
}
 
class Bar extends Foo {
    public static void method() {
        System.out.println("in Bar");
    }
}
```

Both the codes compile and run fine.

But the second one isn't an example of one static method overriding another static method. Its an example of a static method hiding another static method.

What's the difference?

=> [[Runtime Polymorphism -- When you override - you get it -- when you hide - you don't]]

[[Why compiler sometimes talks about overriding static methods]
