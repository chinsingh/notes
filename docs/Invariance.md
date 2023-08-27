# Invariance

Neither component of sub-type nor component of super-type can replace or assigned to each other.

- Example

    ```csharp
    //Lists in C# are invariant
    List<Mango> mangoList = new List<Mango>();
    List<Fruit> fruitList = new List<Fruit>();
    
    mangoList = fruitList; //error
    fruitList = mangoList; //error
    ```
