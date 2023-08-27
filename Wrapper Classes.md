# Wrapper Classes

- There is a wrapper class for every primitive data type in Java. For example, there’s Integer for int, Character for char, Float for float, Double for double and so on. That is, the class names are same as the data types’ name (Except char and int) apart from the fact that the class names begin with uppercase letters, which is a convention in Java.
- We can create objects of these wrapper classes instead of variables of primitive data types.
- Wrapper classes contains one variable (data member) of their respective primitive data type. They also contain certain functions to manipulate these values.
- Why?
  - [[Everything is an Object]]
  - Java — primitive data types ⇒ Not objects ⇒ Wrapper classes
  - Also, to make methods available to operate on primitive data types.
- All wrapper classes are [[immutable class]]es
- All wrapper classes implement [[Comparable]]
