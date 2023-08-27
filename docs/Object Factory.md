# Object Factory

- The single responsibility of an object factory class is to create objects of other classes
- The factory decides if it provides the [[singleton]] or a new object every time
- To prevent unwanted side effects due to the direct creation of the managed classes,

```abap
CLASS cl_managed DEFINITION
    PUBLIC
    CREATE PRIVATE "Define the constructor of the factory-managed class as private
    GLOBAL FRIENDS cl_factory "Declare the factory as a global friend of the factory-managed class
```
