# values(), valuesOf(), ordinal() Functions in [[Java Enums]]

- Functions values(), valueOf() and ordinal() are added by compiler/JVM to the enum

## values()

- Returns all values in the enum in form of an array.
- Usage

```java
Laptop.values(); 
//Output - APPLE,HTC,SAMSUNG

```

## valueOf()

- Returns value of given constant enum
- Usage

    ```java
    Laptops.valueOf("APPLE") 
    //APPLE
    ```

## ordinal()

- Returns index of an enum constant.
- Usage

    ```java
    Laptops.HTC.ordinal() //2
    ```
