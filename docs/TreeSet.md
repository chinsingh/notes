# TreeSet

implements [[NavigableSet]]

- Underlying Data Structure: Balanced Tree
- Duplicates: Not allowed
- Insertion Order: Not preserved
- null insertion: Not allowed
- Best choice for: Cache-based application
- Worst choice for:
- Constructors:
  1. `TreeSet A = new TreeSet()`
  2. `TreeSet A = new TreeSet(Comparator C)`
  3. `TreeSet A = new TreeSet(Collection C)`
  4. `TreeSet A = new  TreeSet(SortedSet S)`
- Default initial capacity: 0
- Load factor/fill ratio:
- New Capacity: Increases as elements are added
