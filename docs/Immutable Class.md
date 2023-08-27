# Immutable Class

Cannot be changed (mutated)

Whenever changed - a new instance is created

## All wrapper classes + String

- String
- Boolean
- Byte
- Short
- Integer
- Long
- Float
- Double

## What makes a class immutable?

- Instance variable is final (value can't be changed)
- class = final - So subclass can't be created
- No setters

## How to create an immutable class

- Create **final** class with all **final data members**.
- You can make a class immutable using builder pattern [[Source](https://www.journaldev.com/1432/java-immutable-class-builder)]

## References

[Java Immutable Class - Builder Pattern](https://www.journaldev.com/1432/java-immutable-class-builder)
