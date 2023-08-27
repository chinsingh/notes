# ArrayList

implements [[List]] and [[RandomAccess]]

- Underlying Data Structure: Resizable Array
- Duplicates: Allowed
- Insertion Order: Preserved
- null insertion: Allowed
- Best choice for: Frequent Retrieval (Random Access)
- Worst choice for: Frequent Insertion/deletion in middle -> Several shift operations are required
- Constructors:
   1. `ArrayList l = new ArrayList();`
   2. `ArrayList l = new ArrayList(int initialCapacity);`
   3. `ArrayList l = new ArrayList(Collection C);`
- Default initial capacity: 10
- Load factor/fill ratio:
- New Capacity: 1.5C + 1

References are stored contiguously (not the objects).
