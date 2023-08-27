# Factory Method

- Goal
  - Classes of more abstract levels shall not depend on classes on more detailed levels
  - Classes shall only depend on abstractions, e.g. interfaces
- Solution

    Move creation of objects to object factory class
    ![Factory class object creation](library/attachments/2022-12-17-05-47-24.png)

- Testability advantage

    Offers a single point of injection for [[Test Double]]s in unit tests and integration/system tests

- Create the Interface and multiple implementation of same interface.
- Factory method - used to hide the logic of object creation  - loose coupling and high cohesion
- Create another class and initialize the object in a method over there. Return the object.
