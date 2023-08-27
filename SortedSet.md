# SortedSet

implements [[Set]]

- Duplicates: NOT allowed
- Insertion Order: Preserved
- Sorting Order: Customizable

| Methods           | Returns                                                                       |
|-------------------|-------------------------------------------------------------------------------|
| - first()         | → first element                                                               |
| - last()          | → last element                                                                |
| - headSet(*a*)    | → elements less than *a*                                                      |
| - tailSet(*a*)    | → elements greater than or equal to *a*                                       |
| - subSet(*a*,*b*) | → elements between *a* and *b* including *a*                                  |
| - comparator()    | → Comparator object which defines underlying sorting technique                |
|                   |   (If we're using default natural sorting order, then it simply returns null) |

Child classes/interfaces:

[[NavigableSet]] (I)
