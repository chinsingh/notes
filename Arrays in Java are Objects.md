# Arrays in Java are Objects

- This is why arrays are initialized using `new` keyword
- For each array type, there exists a corresponding class.
  - So there is a class for int[], for float[], double[] etc.
  - These classes are the part of java language and not available to the programmer level
  - To know the class of any array

    ```java
    // Here x is the name of the array.
    System.out.println(x.getClass().getName());
    ```

- [[Corresponding class names for some array types]]
- Every array type implements [[Serializable]]  and [[Cloneable]] interface
- Arrays can be assigned to variables of type Object — [[Upcasting]].
- All methods of Object class can be invoked on an array

## References

- [Is an array a primitive type or an object in Java? - GeeksforGeeks](https://www.geeksforgeeks.org/array-primitive-type-object-java/)
- [Chapter 10. Arrays - Oracle Docs](https://docs.oracle.com/javase/specs/jls/se7/html/jls-10.html)
