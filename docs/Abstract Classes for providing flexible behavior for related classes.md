# [[Abstract]] Classes for [[providing flexible behavior for related classes]]

If there is a common interface for all concrete implmentations of your abstract class, it means you are just using [[inheritance]] to define/change certain behaviour of the class.

![Abstract class substituting strategy](<../attachments/Abstract Classes for providing flexible behavior for related classes-image.png>)

You should rather prefer [[composition over inheritance]].

Just turn your abstract class into a concrete implementation and inject the "behaviour" which you are trying to change from outside using [[Strategy Pattern]].

![Strategy Pattern instead of Abstract Classes](<../attachments/Abstract Classes for providing flexible behavior for related classes-image-1.png>)

## References

[Nigel Thorne's answer to How to Unit Test Abstract Classes?](https://stackoverflow.com/a/2947823/14318926)

[//begin]: # "Autogenerated link references for markdown compatibility"
[Abstract]: Abstract "Abstract"
[providing flexible behavior for related classes]: <Providing flexible behavior for related classes> "Providing flexible behavior for related classes"
[inheritance]: Inheritance "Inheritance"
[composition over inheritance]: <Composition over Inheritance> "Composition over Inheritance"
[Strategy Pattern]: <Strategy Pattern> "Strategy Pattern"
[//end]: # "Autogenerated link references"