# Exception Handling with Method Overriding

## Case 1: Super class doesn't declare an exception

Sub class overridden method:

- cannot declare a [[Checked Exception]] but
- can declare an [[Unchecked Exception]].

## Case 2: Super class declares an exception

Sub class overridden method

- can declare
  - same exception
  - subclass exception (covariant)
  - or no exception
  but
- cannot declare parent exception
