# Human h = new Student is not dynamic binding

Someone could very easily make an argument that `Human h = new Student()` is not [[Dynamic Binding]]

```java
class Human{
    foo(){}
}

class Student extends Human{
    foo(){}
    xyz(){}
}

main(){
    Human h = new Student();
    
    h.xyz(); //This line will give error. 
    h.foo(); 
}
```

## Why it looks like its not runtime polymorphism

The line `h.xyz()` will immediately show an error.

- `h.xyz()`  shows error
- ⇒ Program doesn't know h is an object of class Student
- ⇒ h is an object of Human type
- ⇒ Its not runtime polymorphism

## What actually happens

Compiler doesn't know at compile time that 'h' is an object of Student type.

- Object type determined at runtime
- ⇒ Compiler still thinks 'h' is an object of Human type
- ⇒ COMPILE TIME Error.
