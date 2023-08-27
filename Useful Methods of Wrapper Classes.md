# Useful Methods of [[Wrapper Classes]]

## valueOf()

- Static Method
- Returns object reference of corresponding wrapper class.
- **Syntax**

    ```java
    WrapperClass reference_variable = WrapperClass.valueOf(“Number in string format”, base-decimal by default);
    ```

- **Example**

    ```java
    Integer i1=Integer.valueOf(“123”);
    Integer i2=Integer.valueOf(“101011”,2);
    Double d1=Double.valueOf(“3.14”);
    ```

## parseXxx()

- Static Method
- Xxx can be replaced with any primitive data type
- Similar to valueOf() but returns reference to xxx type rather than a wrapper class object.
- Syntax

    ```java
    xxx**.**varname = WrapperClass**.**parseXxx(“Number in string format”);
    ```

- Example

    ```java
    int a=Integer.parseInt(“123”);
    double b=Double.parseDouble(“13.45”);
    ```

## xxxValue()

- Instance method
- Xxx can be replaced with any primitive data type
- Returns corresponding primitive data type.
- Used to convert from/get the value of a wrapper class object to a primitive data type.
- **Syntax**

    ```java
    xxx varname=objectname.xxxValue();
    ```

- **Example**

    ```java
    //i1 contains a reference of object of Integer class.
    int c = i1.intValue();
    ```
