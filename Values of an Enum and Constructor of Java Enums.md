# Values of an Enum and Constructor of [[Java Enums]]

Compiler adds a constructor to the enum. We can enter custom values for enums too.  We need to create a parameterized constructor for that.

- Example

    ```java
    enum  Fruits
    {
        APPLE(“RED”), BANANA(“YELLOW”), GRAPES(“GREEN”);
    }
    ```

    Thus, the value of enum APPLE is not "APPLE". It is "RED" instead.

    ```java
    //Example
    enum Mobile { 
    int price;
    APPLE(1200), SAMSUNG(700), HTC(400);
    Mobile(int p){ price = p} //Constructor
    }
    ```

- Although, the constructor is private and hence, enums can't be initialised by new().
