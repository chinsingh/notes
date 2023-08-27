# [[Static Method]]s can't be overridden

You can't.

```java
//Can't do this -> Compile time error
class Foo {
    public static void method() {
        System.out.println("in Foo");
    }
}
 
class Bar extends Foo {
    public void method() {
        System.out.println("in Bar");
    }
}
```

[[Why compiler sometimes talks about overriding static methods]]
