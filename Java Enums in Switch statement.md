# [[Java Enums]] in Switch statement

Switch statement cases can only include values which are in enum.

```java
enum Laptop{ APPLE, DELL, SAMSUNG }
.
.
.
Laptop l = Laptop.SAMSUNG; //Creating object of enum
switch(l){
    case APPLE:
    case SAMSUNG:
    case LUDO: //Will give error.
}
```
