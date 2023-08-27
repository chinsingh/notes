# Order of invokation of initialization blocks and constructors

Parent static block
Child static block
Parent initialization  block
Parent Constructor
Child initialization block
Child Constructor

👆🏽 output of the code below

```java
public class Parent {    
    public Parent() {
        System.out.println("Parent Constructor");
    }    
    static {
        System.out.println("Parent static block");    
    }    
    {
        System.out.println("Parent initialisation  block");
    }
}

public class Child extends Parent {    
    {
        System.out.println("Child initialisation block");
    }
    static {
        System.out.println("Child static block");
    }

    public Child() {
        System.out.println("Child Constructor");
    }    
    public static void main(String[] args) {
        new Child();    
    }
}
```

Initialization blocks get invoked in the order they're written in the code.

## References

- [In what order do static blocks and initialization blocks execute when using inheritance? - Stack Overflow](https://stackoverflow.com/questions/19561332/in-what-order-do-static-blocks-and-initialization-blocks-execute-when-using-inhe)
- [Order of execution of Initialization blocks and Constructors in Java](https://www.geeksforgeeks.org/order-execution-initialization-blocks-constructors-java/#:~:text=Initialization%20blocks%20run%20in%20the,above%20the%20constructors%20within%20braces.)
