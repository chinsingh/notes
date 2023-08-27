# null vs empty String

```java
String getSome;
String getMose = "";
```

Both of them are not the same. "" is a literal and has a reference pointing to it in the String constant pool, while getSome has no value/reference in it so its null → default value for String.
