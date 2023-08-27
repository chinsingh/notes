# Contravariance

- Opposite of [[Covariance]]
- If the component of sub-type can be replaced with by component of super-type, it is called covariance.

    Or

    Component of super-type can be assigned to component of sub-type.

```csharp
static void GetFruitInfo(Fruit fruit){}
static void GetMangoInfo(Mango mango){}

main(){

Action<Fruit> fruitInfo = GetFruitInfo;
Action<Mango> mangoInfo = GetMangoInfo;

fruitInfo = mangoInfo; //error
mangoInfo = fruitInfo;
}
```
