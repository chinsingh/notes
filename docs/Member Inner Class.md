# Member Inner Class

If class B is inside class A

```java

main()
{ 
A obj = new A();
A.B obj1 = obj.new B();
}

//If j is member of class B
obj1.j=5;
```

`.class` files in this case:

`A.class`
`A$B.class`
