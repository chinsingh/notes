# [[Dependency]] Injection

```abap
CLASS … DEFINITION … .
 DATA(lo_cash_provider) = NEW cl_cash_provider( ).
ENDCLASS
```

👆🏽 This here is a [[Dependency]]

- Dependency injection is a design pattern in which, instead of creating the object ourselves in our code, we let some other entity create the object and "inject" into our class.
- ⇒ Dependency injection implements [[Inversion of Control (IoC)]]

[[Constructor Injection]]
[[Setter Injection]]
[[Parameter Injection]]
[[Backdoor Injection]]
