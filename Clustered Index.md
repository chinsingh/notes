# Clustered Indexing

- Database is sorted but indexing is done on non-key attribute.
- Thus, search key used here is not unique and hence the name.
- Clustered indexes can have [[Sparse Index]]ing and [[Dense Index]]ing at the same time.
  - Consider a table with a field which has values  1,1,1, 2, 3, 3, 4, 5
  - When you index over this key, you store the keys — 1, 2, 3, 4, 5
  - You stored keys for all values — dense
  - You didn't store for all records — sparse
