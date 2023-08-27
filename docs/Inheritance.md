# Inheritance

Mechanism through which an object acquires all the properties and methods of its parent

## Implemented by

`extends` keyword

## What kind of relationship?

IS - A

## What is inherited?

💡 By inherited, it is meant that these fields and methods are part of of the subclass, as if the subclass had declared them itself.

When a subclass inherits a superclass, all protected and public fields and methods of the superclass are inherited by the subclass.  Protected and public fields can be called and referenced just like the methods declared directly in the subclass.

Private fields and methods of the superclass can never be referenced directly by subclasses. They can, however, be referenced indirectly via methods reachable from the subclass (e.g default (package), protected and public methods).

## Types of Inheritance

- [[Single Inheritance]]
- [[Multilevel Inheritance]]
- [[Multiple Inheritance]]
- [[Hierarchical Inheritance]]
- [[Hybrid Inheritance]]
