# Getting Objects of Cursors in Java

- Enumeration, Iterator, ListIterator are all interfaces
- How can we create objects for interfaces then?
    ⇒ We don't.

    What happens actually, is that the elements() method has a class within it which implements Enumeration interface. elements() returns the object of that class. This is how it works for other two cursor interfaces as well.

    ```java
    System.out.println(c.getClass().getName()); //c is an object of a cursor
    ```

    ```java
    Output
    
    vector$1              // if c is an Enumeration Object
    vector$Itr            // if c is an Iterator Object
    vector$ListItr        // if c is a List Iterator Object
    ```

    vector$ means inner class of vector ( or whichever Collection class we're getting the object for)

    1 means it is an anonymous inner class

    Itr and List Itr are names of inner classes implementing Iterator and ListIterator respectively.
