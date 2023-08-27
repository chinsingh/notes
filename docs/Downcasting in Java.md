# [[Downcasting]] in Java

## Syntax

- Same as narrowing conversion in primitive data types

    ```java
    float a = 10.5;
    int b = (int) a;

    print(a) -→ 10.5
    print(b) -→ 10
    ```

- Another way

    ```java
    Animal animal = new Animal();
    if (Cat.class.isInstance(animal)) {
    Cat cat = Cat.class.cast(animal);
    ```

## [[Class Cast Exception]] — ClassCastException

That is why it is advised to use *instanceOf* check before downcasting.

- instanceOf

    Used to avoid the ClassCastException by checking if the object belongs to a certain type

    ```java
    //Example 
    if (animal instanceof Cat) {
        ((Cat) animal).meow();
    }
    
    ```

    ```java
    //case 1
    Dog dog = new Dog();
    Animal animal = dog;

    if(Cat.class.instanceOf(animal)) -→ false

    //case 2
    Cat cat = new Cat();
    Animal animal = cat;

    cat.meow();

    Cat.class.instanceOf(animal) -→ true
    ```
