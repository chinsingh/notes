# Covariance

If the component of super-type can be replaced with by component of sub-type, it is called covariance.

Or

Component of sub-type can be assigned to component of super-type.

For example, if list of animals can be replaced by list of cats.

```csharp
IEnumerable<Mango> mangoes = new List<Mango>();
IEnumerable<Fruit> fruits = new List<Fruit>();

mangoes = fruits; //wrong - error
fruits = mangoes;
```
